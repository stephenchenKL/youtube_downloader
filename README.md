# youtube_downloader

setuptools 60.2.0

pip 21.3.1

pytube 15.0.0

PyQt5-sip 12.12.1

PyQt5 5.15.9

PyQt5-Qt5 5.15.2

typing-extensions 4.6.0

wheel 0.37.1


Error:
pytube.exceptions.RegexMatchError: __init__: could not find match for ^\w+\W

Solution:
go in the cipher.py file and replace the line 30, which is:
var_regex = re.compile(r"^\w+\W")
With this line:
var_regex = re.compile(r"^\$*\w+\W")
