## Flat page edits

### Sphinx Navbar

- See https://github.com/IQSS/dataverse.org/tree/master/dataverse_org/templates/sphinx-navbar

### Log into the admin

- http://beta.dataverse.org/dataverse-org-admin/

### Create Flat page

- Click on "Flat pages"
- Add/edit/delete
- *Remember the url* that you enter.
    - Example ```/history-and-name/```
- [screenshot: edit page](https://github.com/IQSS/dataverse.org/blob/master/dataverse_org/static/images/user_notes/flatpage_edit.png)
- [screenshot: view page](https://github.com/IQSS/dataverse.org/blob/master/dataverse_org/static/images/user_notes/flatpage_view.png)

### Link your page to the menu

- Edit the [navbar.html](https://github.com/IQSS/dataverse.org/blob/master/dataverse_org/templates/navbar.html) file
- Add the your url to the appropriate place. Example:

```
<li><a href="/history-and-name/">History &amp; Name</a></li>
```
- To have this template show up on the live site, run the jenkins build (about 10-20 seconds)
- [screenshot: nav bar, highlight active link](https://github.com/IQSS/dataverse.org/blob/master/dataverse_org/static/images/user_notes/flatpage_navbar.png)

### Add an image to the repository ("static/images")

- On your local machine, place your image in the ["static/images"](https://github.com/IQSS/dataverse.org/tree/master/dataverse_org/static/images) directory
- Sync github (to upload to github)
- To have this image available on the live site, run the jenkins build (about 10-20 seconds)

### Link your image in a flatpage ("static/images")

- Assumption: your image is checked into the repository under "static/images" (described above)
- In the flat page content box, use this syntax:

```
<img src="/static/images/your-image-name.png" alt="description" />
````

