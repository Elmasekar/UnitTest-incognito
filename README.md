# How to run an automation test in incognito mode in UnitTest on [LambdaTest](https://www.lambdatest.com/?utm_source=github&utm_medium=repo&utm_campaign=UnitTest-incognito)

If you want to run you automation test in UnitTest in incognito mode on Lambdatest, you can use the following steps. You can refer to sample test repo [here](https://github.com/LambdaTest/Python-UnitTest-Selenium).

# Steps:

You can specify the incognito option in the test file capabilities. The following is an example on how to set incognito option using chromeOptions:

```python
desired_caps = {
            'LT:Options': {
                "build": "Python Demo",  # Change your build name here
                "name": "Python Demo Test",  # Change your test name here
                "platformName": "Windows 11",
                "selenium_version": "4.0.0",
                "chromeOptions" : {
                "args" : ["incognito"]  # ChromeOption to start chrome in incognito mode
                }
            },
            "browserName": "Chrome",
            "browserVersion": "98.0",
        }

```

## Run your test

```bash
python lambdatest.py
```

# Links:

[LambdaTest Community](http://community.lambdatest.com/)
