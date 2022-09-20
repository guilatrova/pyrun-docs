# Creating content

Here's a few examples on how to make it work:

## Twitter

![type:video](./videos/creating-on-twitter.mp4)

## Facebook

![type:video](./videos/creating-on-facebook.mp4)

## Linkedin

![type:video](./videos/creating-on-linkedin.mp4)

## Linkedin images with up to 1000 characters ALT


!!! warning
    Linkedin limits image's ALT to 300 characters.
    You can overcome this limit by modifying your HTML.

If you need to share snippets with more text, you can literally just modify the HTML just **like a Ninja** 🥷.

Take as example this 532 length code:

```py title="long_snippet.py"
from typing import Generator

def starting_five() -> Generator[int, None, None]:
    """Generator that returns integers from 1-5"""
    for n in range(1, 6):
        yield n


def ending_five() -> Generator[int, None, None]:
    """Generator that returns integers from 6-10"""
    for n in range(6, 11):
        yield n


def all_ten() -> Generator[int, None, None]:
    """Generator that relies on other generators"""
    yield starting_five() # 👈 This is broken
    yield ending_five()  # 👈 This is broken


print(list(all_ten()))
```

Here's what you should do:

![type:video](./videos/creating-on-linkedin-more-characters.mp4)
