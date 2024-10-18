---
layout: post
title: "Setting Up Python in VSCode"
---

It might be your first time using **VSCode**, so don't worry; setting it up can be a bit tedious.

In this case, we want to use it for **Python** development, so we will need to adapt it for that purpose.

### Extensions
If we click on the **Extensions** section on the left side, a search bar will appear at the top. We type **"Python"** into it. All the installable extensions in VSCode will appear for customizing our IDE. We just need to click on **"Install"** to proceed with the installation (see image).

However, a fundamental part (without which none of this would work) is to have the **Python** interpreter downloaded on our PC. To do this, we would go to the **"Software Center"** from step 2 and download the latest available version of **Python**. It is also possible to download it from the official Python website.

![Image Description]({{ site.baseurl }}/images/interprete-python.png)

### Interpreter
Once installed, we need to tell **VSCode** which interpreter we want to use. To do this, we click on the bottom left corner of the **VSCode** window (in orange in the image), and a list will drop down in the top center. We will click on **"Enter interpreter path…"** and then enter the path where our interpreter is located.

But where is it? It has likely been installed in the following path: **“C:\Program Files (x86)\Python38-32”**, or a similar path on your PC.

It is also possible that **VSCode** has detected multiple interpreters on your PC, allowing you to select one directly from the list provided instead of entering the path manually.

Installing libraries should be as simple as entering this text in **CMD** or the **VSCode** Terminal:

```bash
pip install library_name
```

However, life isn't always that easy. It might not work for you. Here are several options to try to fix it:

- If you get an error like “ERROR: Could not install packages due to an EnvironmentError”, it is because you are connected via cable to the Alstom network (it won't let you download anything). Therefore, you will need to use a USB Internet Stick.

- You might need to run CMD as an administrator.

- You may have to add the path to Python in the system variables:

Windows+E > "This PC" (right-click) > Properties > Advanced system settings (you will need admin permissions) > Advanced options > Environment Variables > Path (edit) -> paste the path of the Python interpreter.