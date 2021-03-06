# Overview

The Export User Data plugin for Movable Type allows administrators to export
all of the information collected about their site's users into a
comma-separated format (.csv) file.

# Prerequisities

* Movable Type 5.1+
* [Config Assistant 2.5.7+](https://github.com/openmelody/mt-plugin-configassistant/releases)

Movable Type 4.x is supported with [version 1.1](https://github.com/endevver/mt-plugin-userexport/releases).

# Installation

To install this plugin follow the instructions found here:

[http://tinyurl.com/easy-plugin-install](http://tinyurl.com/easy-plugin-install)

# Usage

System administrators will find an "Export user data" Page Action on the
system-level Users screen. Click this to get started!

On the **Filter** screen you can home-in on the users you want, then click the
Select Fields button to continue:

* Select the user's status. "Enabled" and "disabled" are clear options.
  "Pending" users are those who have registered with Movable Type, but who
  have not confirmed their registration.
* Select the user's role. This list allows multiple selections, and is most
  useful for specifically accessing your users, who likely have either the
  Commenter or Contributor role. Alternatively, by selecting Author, Editor,
  and Moderator you can generate a list of your site's administrative team,
  for example.
* Select the blog(s) to export from. If your Movable Type install runs
  multiple domains, being able to export user data for specific blogs is
  important.
* By default, only users who have used MT authentication will be exported,
  because those are the users with the most useful data. (Custom fields, for
  example, can only be filled-in by MT-authenticated users.) If you want to
  export the data from users who have authenticated through other methods such
  as TypePad or Facebook, in addition to those authenticated through MT, check
  this checkbox.

The Filter screen continues, where you can filter based on author Custom
Fields. Select one or more custom fields to filter on, then select how these
fields should be used:

* Users with matching custom field data for the selected fields should be
  exported. That is, if a user profile contains a value for the selected
  field, that user will be exported.
* Users with matching custom field data for the selected fields should *not*
  be exported. That is, if a user profile contains a value for the selected
  field, that user will *not* be exported.

On the **Fields** screen you will find a table of author profile fields,
including any custom fields that may be defined. Place checkmarks next to the
fields that you want to include in your export data. Click and drag fields to
re-arrange their order. Note that the User ID field will always be exported,
and can not be reordered. Click the Export button to continue; depending upon
the size of the dataset, this may take a few moments.

If you are using the [Download Genie](https://github.com/endevver/mt-plugin-download-genie) plugin, and if
statistics recording is enabled within Download Genie, you have some
additional options: the total number of files downloaded and the downloaded
file name, date, and time can also be exported. Note that exporting the
downloaded file name, date and time can result in a lot of additional data
being exported.

Lastly, on the **Export** screen you're presented with the result! The file
name, location, and size are reported here, as is a link to download the data.
If you've enabled the Display Export Results option, you also see your
exported data here.

The resulting comma-separated file can be imported and analyzed with Numbers
or Excel or other spreadsheet application!

Notice that the options chosen to create the exported data is saved, so the
next time you need to export your preferences are re-used!

# Acknowledgements

This plugin was commissioned by Endevver to Dan Wolfgang of uiNNOVATIONS.
Endevver is proud to be partners with uiNNOVATIONS.

http://uinnovations.com/

# License

This plugin is licensed under the same terms as Perl itself.

# Copyright

Copyright 2009, Endevver LLC. All rights reserved.
