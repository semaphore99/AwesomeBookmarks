# C#
- [Async constructors](https://blog.stephencleary.com/2013/01/async-oop-2-constructors.html)

- [Fire and Forget tasks](https://stackoverflow.com/questions/12803012/fire-and-forget-with-async-vs-old-async-delegate)
- [Another fire and forget article ](https://johnthiriet.com/removing-async-void/)
- [Returning void from C# async methods](https://app.pluralsight.com/guides/returning-void-from-c-async-method)
- [Xamarin Application Themes](https://docs.microsoft.com/en-us/xamarin/xamarin-forms/user-interface/theming/theming)
- [Data validation using IDataErrorInfo](https://www.codeproject.com/tips/858492/wpf-validation-using-idataerrorinfo)
- [Timing out a block of code](https://stackoverflow.com/questions/13513650/how-to-set-timeout-for-a-line-of-c-sharp-code)
- ObservableCollection is not thread-safe, so here are some solutions:
  - [Thread-safe ObservableCollection (WPF solution)](https://stackoverflow.com/questions/23108045/how-to-make-observablecollection-thread-safe)
  - [SynchronizedObservableCollection from CodeProject](https://www.codeproject.com/tips/998619/thread-safe-observablecollection-t) - note this solution uses ```SynchronizationContext.Send()```, which has been deprecated so [this solution](https://stackoverflow.com/questions/22441499/replacement-for-synchronizationcontext-send-in-portable-class-libraries) to replace the ```.Send()``` calls.
