# C#
## Async Programming
- [Async constructors](https://blog.stephencleary.com/2013/01/async-oop-2-constructors.html)
- [Fire and Forget tasks](https://stackoverflow.com/questions/12803012/fire-and-forget-with-async-vs-old-async-delegate)
- [Another fire and forget article ](https://johnthiriet.com/removing-async-void/)
- [Returning void from C# async methods](https://app.pluralsight.com/guides/returning-void-from-c-async-method)
- [Timing out a block of code](https://stackoverflow.com/questions/13513650/how-to-set-timeout-for-a-line-of-c-sharp-code)
- [Dispatcher.CurrentDispatcher vs. Application.Current.Dispatcher](https://stackoverflow.com/questions/10448987/dispatcher-currentdispatcher-vs-application-current-dispatcher)

## Xamarin.Forms
### Architecture
- [Enterprise Application Patterns](https://docs.microsoft.com/en-us/xamarin/xamarin-forms/enterprise-application-patterns/)
### Theming
- [Xamarin Application Themes](https://docs.microsoft.com/en-us/xamarin/xamarin-forms/user-interface/theming/theming)
### Debugging
- [Connecting to locally hosted web services from emulators](https://docs.microsoft.com/en-us/xamarin/cross-platform/deploy-test/connect-to-local-web-services)

## WPF
- [Data validation using IDataErrorInfo](https://www.codeproject.com/tips/858492/wpf-validation-using-idataerrorinfo)
- [WPF binding cheatsheet](https://www.nbdtech.com/Free/WpfBinding.pdf)
### Commands
- [Force update commands](https://stackoverflow.com/questions/783104/refresh-wpf-command) - note this has a performance penalty since it refreshes **ALL** commands and must be called from the UI thread.
- [Command that 'binds' to a property](https://stackoverflow.com/questions/1751966/commandmanager-invalidaterequerysuggested-isnt-fast-enough-what-can-i-do)
  
 ### App icon in system tray
 - [WPF application with system tray icon - this uses a WinForms API but works](https://stackoverflow.com/questions/1472633/wpf-application-that-only-has-a-tray-icon)
 - [Windows applicatio nnotify icon Context menus](https://docs.microsoft.com/en-us/dotnet/api/system.windows.forms.notifyicon.contextmenu?view=netframework-4.8)
 - [C# tray icon using wpf](https://stackoverflow.com/questions/12428006/c-sharp-trayicon-using-wpf): this was a nice a simple solution that I ended up using
 - [Context menus on tray icon (doc.microsoft)](https://docs.microsoft.com/en-us/dotnet/api/system.windows.forms.notifyicon.contextmenu?view=netframework-4.8)
 
### Targetting another app Window
This got pieced together from a few different sources:
- [Find a target window and minimize, maximize, or restore it in C#](http://csharphelper.com/blog/2016/12/find-a-target-window-and-minimize-maximize-or-restore-it-in-c/)
- [How to get and set the window position of another application in C#](https://stackoverflow.com/questions/1364440/how-to-get-and-set-the-window-position-of-another-application-in-c-sharp): Answer from mkelement0 was quite instructive
- [SetWindowPos function (doc.microsoft)](https://docs.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-setwindowpos)

## General
- ObservableCollection is not thread-safe, so here are some solutions:
  - [Thread-safe ObservableCollection (WPF solution)](https://stackoverflow.com/questions/23108045/how-to-make-observablecollection-thread-safe)
  - [SynchronizedObservableCollection from CodeProject](https://www.codeproject.com/tips/998619/thread-safe-observablecollection-t) - note this solution uses ```SynchronizationContext.Send()```, which has been deprecated so [this solution](https://stackoverflow.com/questions/22441499/replacement-for-synchronizationcontext-send-in-portable-class-libraries) to replace the ```.Send()``` calls.
  - [Visual Studio Magazine](https://visualstudiomagazine.com/Home.aspx)
- [IQueryable vs IEnumerable](https://stackoverflow.com/questions/2876616/returning-ienumerablet-vs-iqueryablet)
  
## Logging
- [How to get the stack frame](https://www.csharp-examples.net/reflection-callstack/)
- [NLog](https://github.com/NLog/NLog)

# Couchbase
- [Couchbase.Lite API for C#](https://docs.couchbase.com/couchbase-lite/current/csharp.html)

# Identity
- [Learn Identity video series from Auth0](https://auth0.com/docs/videos/learn-identity-series)
- [Auth0 quick starts](https://auth0.com/docs/quickstarts)
- [Secure a .NET Core 3.0 Web API](https://auth0.com/blog/how-to-build-and-secure-web-apis-with-aspnet-core-3/)
- [Authentication with Xamarin Forms and Auth0](https://purple.telstra.com/blog/authentication-with-xamarin-forms-and-auth0)

# General
- [Example class design for messenger/chat](https://github.com/yoosuf/Messenger)
