# NetFrameworkRazorDoubleInputBug

This repository can be used to reproduce an issue in **Visual Studio 17.12** that causes double input when editing a **.cshtml** file in a **.NET Framework** project with **GitHub Copilot Completions** enabled.

Here is a video showcasing the issue:

https://github.com/user-attachments/assets/822f7e7b-73e2-4d79-a6db-d521df89a870

## Notes:

- The issue causes double input when typing in a .cshtml file. E.g. typing "hello" results in "hheelllloo".
- The issue seems to occur when GitHub Copilot Completions are enabled. After disabling GitHub  Copilot Completions, the issue no longer occurs.
- This project was created with the default "ASP .NET Web Application (.NET Framework)" template in VS 17.12 with .NET Framework 4.8.1.
    - The template is included if VS was installed with component ".NET Framework project and item templates" selected in VS Installer (under "individual components").
- This issue may occur under other conditions, too.
