# How to navigate between views in NavigationFrame


<p>This example demonstrates how to navigate between views without executing code at the view model level. If you wish to control navigation from the view mode, please refer to: <a href="https://www.devexpress.com/Support/Center/p/E4697">How to: Navigate between Views via FrameNavigationService</a>.<br><br>In this example, the NavigationButton element is used to perform navigation. To specify the target view, use the NavigateTo property. If you wish to use the standard Button, set the dxwuin:Navigation.NavigateTo attached property:</p>


```xaml
<Button Content="Tools" dxwuin:Navigation.NavigateTo="ToolsView"/>
```


<p>Please note that the approach with the NavigationButton and Navigation.NavigateTo properties works only if the button is located in the NavigationFrame's visual tree.  You can also use the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfWindowsUINavigationFrame_Navigatetopic(IuWGjg)">NavigationFrame.Navigate</a> method to initiate navigation from code-behind. To specify the start view, set the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfWindowsUINavigationFrame_Sourcetopic">Source</a> property.</p>
<p><br>In this example, each view contains the PageAdornerControl. This element consists of a header and a back button. As a rule, the header is used for navigation buttons and for displaying the view name. The back button is visible only when the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfWindowsUIPageAdornerControl_ShowBackButtontopic">ShowBackButton</a> is true.<br><br></p>
<p>To cache views in order to improve performance, set the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfWindowsUINavigationFrame_NavigationCacheModetopic">NavigationCacheMode</a> to "Required".</p>

<br/>


