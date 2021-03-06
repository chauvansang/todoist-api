# Introduction

Welcome to the official Todoist API documentation!  The Todoist API can be used to hook [Todoist](https://todoist.com) with other applications, as it makes it easy for your client to retrieve and sync your data.

The Todoist API is based on [REST](http://en.wikipedia.org/wiki/Representational_State_Transfer), so you can use it with a tool like [cURL](http://curl.haxx.se), but language bindings also exist for [Python](https://www.python.org), so it is easier and faster to write your own scripts or applications interacting with Todoist.

The [source code](https://github.com/Doist/todoist-api) of this API documentation is also available.

## Libraries

### Python

> You can install the Todoist Python library from PyPI with:

```
$ pip install todoist-python
```

At the moment there are language bindings for Python, in the form of the [Todoist Python API library](https://github.com/Doist/todoist-python).

A [PyPI package](https://pypi.python.org/pypi/todoist-python) has been also prepared in order to easily install the Todoist Python library in your system.

There is more detailed documentation speficically for the Todoist Python API library, and this [API reference](http://todoist-python.readthedocs.org/en/latest/) documentation can be also read online.

## Overview

The API has been simplified (in version 6), and almost all interactions with
the Todoist server can be done with a single call, which can be used to get the
full model (projects, items, etc.), and then update it, or perform changes to
it.

Then there are a few more auxiliary calls that can perform some actions that
are not related to the full model, but are nonetheless useful.

### Available calls

Call | Description
---- | -----------
login | Logins to the server using the user's password.
login_with_google | Logins to the server using OAuth2.
sync | Retrieves or sends data.
upload_file | Uploads a file.
query | Query after date, priority or labels.
register | Registers a new account.
delete_user | Deletes an existing account.
get_redirect_link | Gets the redirect link.
get_productivity_stats | Gets the productivity stats.
update_notification_settings | Updates the notification settings.
get_all_completed_tasks | Gets the user's completed tasks.
add_item | Adds a new item.
