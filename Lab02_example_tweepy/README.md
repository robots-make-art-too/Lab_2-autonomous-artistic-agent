# HOW DO I WORK?

This file is a quick start guide. 

## Initial requirements 

You will first need to activate an account:
1. activated twitter account
2. activated developer account [developer site](https://developer.twitter.com/)
3. have registered for API access
4. have created a project (requires your info and to fill in the forms)
5. then generate your keys and tokens
   - write them down! they display once then never again!

### OOP

- a Tweet is an `Object`
- it has root-level `Attributes` (i.e., id, created_at)
- Tweet `Objects` are the `parent` `Class`
- there can be `children` (i.e., user, place (if geo-tagged))

### JSON OBJECTS

- we are handling JSON data as accessed from twitter
- these are a mix of `Attributes` and `child` `Objects`

---

## Python file setup

The included files need you to update them:
1. file.txt
   - replace each line with the keys and tokens as indicated
2. tweepy_get_info.py
   - replace __CodeBot__ with you bots user name
3. confirm_cam.py
   - replace '/dev/video#' with the path to your camera access
4. shortandtweet.py
   - replace VideoCapture(#) with the number that is associated with your camera
   - replace or change any file names, or file locations
   - replace statusMessage with your desired message
   - replace img/Frame.png with your desired media 
     - OR remove media and change line to API.update_status(statusMessage)


### To consider

The API.update_status() is a `Method`. It has syntax of the form:

```Python
API.update_status(parameters)
```

This `Method` returns an `Object` of `Class` _Status_. Here is a list of its `Parameters`:

- _status_
- _in_reply_to_status_id_
- _attachment_url_
- _media_ids_
- _possibly_sensitive_
- _lat_
- _long_
- _place_id_
- _display_coordinates_

---

## How to run

Examples on how to run the sample `.py` file. Don't forget you can download, install, and use a `Python` specific `IDE`. We talked about these in `Week 02` .. I currently have the `Spyder` `Python IDE` installed.

### Linux/Ubuntu

Can probably just `CTL ALT + T` to open a terminal. Then `cd /path/to/where/python/file/is`. Then: 

```Terminal
python3 tweepy_get_info.py
```

```Python
# in Spyder

```

### macOS



### VSCode on Windows


