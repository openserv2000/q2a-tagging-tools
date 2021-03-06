
Tagging Tools plugin for Question2Answer
=================================================

This is an event plugin for popular open source Q&A platform, [Question2Answer](http://www.question2answer.org). It allows you to select 'tag synonyms' - unwanted or duplicate tags that should be changed or removed.

For example if you had `websites` as a tag, some users may tag a question with `website` instead. With this plugin you can set `website` to always be changed to `websites` when a user enters it.



Installation & Usage
-------------------------------------------------

1. Download and extract the files to a subfolder such as `tagging-tools` inside the `qa-plugins` folder of your Q2A installation. Since the Github repo is updated regularly, a stable versioned package is also provided, e.g. `Q2A-Tagging-Tools-1.5.zip`

2. Log in to your Q2A site as a Super Administrator and head to Admin > Plugins.

3. Under "Tagging Tools", enter each pair of tags on a new line, separated by a comma. For example, `q2a,question2answer` (without quotes) means that a tag of `q2a` will be replaced by `question2answer`, while `help` on its own line means that tag will be removed.

4. Click the button to save changes. All future questions will replace your chosen tag synonyms.

5. If you have existing mistagged questions, tick the checkbox to replace all tags in older questions with your synonyms.
   WARNING: if you have a lot of questions on your site, converting all the old questions will take a long time. Version 1.5 now uses AJAX to edit a few posts at a time, however, it may still cause high MySQL and Apache CPU usage. It's recommended that you add tag synonyms a handful at a time to avoid too much overhead.

6. The option "Prevent new users from creating new tags" adds a Javascript barrier preventing low-rep users from creating new tags. Currently there is no way to replicate this on the server side without hacking the core, but that will rarely be a problem.



Pay What You Like
-------------------------------------------------

Most of my code is released under the open source GPLv3 license, and provided with a 'Pay What You Like' approach. Feel free to download and modify the plugins/themes to suit your needs, and I hope you value them enough to make a small donation of a few dollars or more.

### [Donate here](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4R5SHBNM3UDLU)
