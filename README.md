# phoneinfoga-google-driver

By default, the Google search scanner doesn't scan links but simply generate them. This driver is intended to complete the job. You may ask, why not including this in the existing project ? Because the default beharvior of PhoneInfoga should be simple and easy to handle. Installing Chromium web driver add some level of complexity which I want to avoid.

## Install

You don't need to install Phoneinfoga first, just [get the binary](https://github.com/sundowndev/phoneinfoga-google-driver/releases).

Or, install using Go get :

```
$ go get github.com/sundowndev/phoneinfoga-google-driver
```

## Usage

```
$ phoneinfoga-google-driver "+1 555-444-6666"
```

It should then use Chromium to scan links then send results in the CLI. If a captcha occurs, a non-headless window will pop up and you'll need to complete captcha.
