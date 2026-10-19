# Kapasan Heritage: app settings

This public repository holds one file, `config.json`, which the Kapasan Heritage Android app reads when it opens.
Edit the file on GitHub (pencil icon > Commit changes) and every phone picks up the change the next time the app is opened online. No rebuild or reinstall is needed.

Keep this repository public and put no private information in it.

| Field | What it does |
|---|---|
| `schema` | Leave as `1`. |
| `site_url` | Address of the website opened by "Open Virtual Tour". Must be https on labsta-its.org, labsta-its.wixsite.com or klapty.com. |
| `survey_id_url`, `survey_en_url` | Indonesian and English survey forms. Must be https on forms.gle or Google Forms. |
| `announcement.text_id`, `announcement.text_en` | Short notice shown at the top of the home screen (up to 300 characters). Leave empty for no notice. |
| `update.latest_version_code` | Number of the newest app version (the `versionCode` in the app). A notice appears only on phones with a lower number and only when `url` is filled. |
| `update.latest_version_name` | Text shown in the notice, for example `1.2.0`. |
| `update.url` | Where to download the new version (Google Play or GitHub release). Must be https on play.google.com, github.com or labsta-its.org. |
| `about.body_id`, `about.body_en` | Replaces the description on the About screen (up to 1,500 characters). Leave empty to keep the built-in text. Credits and copyright stay built into the app. |

If a value is empty, invalid, or the file cannot be read, the app uses its built-in defaults.
Keep the file valid JSON: straight quotes, a comma after every line except the last in a block.
Check it at https://jsonlint.com before committing.
