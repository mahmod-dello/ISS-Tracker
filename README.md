# ISS (International Space Station) Tracker

<img src="iss_image.jpg"  alt="ISS Image"/>

## Project Description

<hr>
This project can send you a notification via email when the International Space Station (ISS) is passing over your country. 
This is achieved by measuring the distance between the latitude and longitude of your location and those of the ISS, 
and then triggering an email notification to be sent to you.

## Required Packages/Modules

<hr>

You can find the required packages/modules used in this project in the [requirements.txt](./requirements.txt) file.
The file contains a list of all the necessary packages and their versions that need to be installed to run the project
successfully.

## Instructions

<hr>

<ol type="I">
<li>Clone the repository.</li>
<li>Setup your venv (Virtual Environment).</li>
<li>You can use <a href="https://latlong.net">latlong </a> to get your latitude and longitude.</li>
<li>Specify the email you want to use as a service:
    <ol type="1">
        <li>Activate 2FA (Two-Factor Authentication).</li>
        <li>Generate an App Password.</li>
        <li>Save the App Password to your ".env" text file.</li>
        <li>Finally you should know your email "smtp" provider. e.g: gmail -> "smtp.gmail.com".</li>
    </ol>
</li>
</ol>

## Bonus

<hr>

1 - When creating this project, I followed a good practice of working with environment variables to hide my personal
information when publishing the project to the public.
To achieve this, I used a Python package called ```python-dotenv``` and set up the ```.env``` text file in a different
directory from the project,
and later on you can access your information using the built-in ```os``` module.
This approach allows you to hide all your personal information, such as emails, passwords, API keys, etc.; that you do
not want to be accessed by the public.
I recommend that you also follow this practice when working on your own projects.

### Example about organizing .env text file:

```
[MyProject]
# My top-secret settings for MyProject
MyUsername="Fred Bloggs"
MyEmail="fred@example.com"
MyPassword="fvghtyu7i890ol"
 
[MyOtherProject]
# My top-secret settings for MyOtherProject
MyAPIKey_MyOtherProject="FMu4ejyK-qQLBasTs7iHx*SFN5F"
email_port=110
DEBUG=True
```

2 - Make your Python code run on the cloud:
Instead of leaving your code running 24/7 on your local machine, 
you have the option to utilize [PythonAnywhere](https://www.pythonanywhere.com/) 
and schedule a task to run every minute on their cloud servers.

# APIs Used in this project
<hr>

[ISS Tracker API](https://open-notify.org/)
<br>
[Sunrise-Sunset API](https://sunrise-sunset.org/api)

# Finally
<hr>

I appreciate you taking the time to read and view this project. Please take care and stay safe.



