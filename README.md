# Xamarin.ActionSheet
Xamarin.Android实现IOS UIActionSheet效果

改写项目：https://github.com/baoyongzhang/android-ActionSheet

只是保证项目能够运行，并没有全部根据C#编码规范重写所有代码。

使用：
设置样式支持IOS6和IOS7
SetTheme (Resource.Style.ActionSheetStyleiOS7);
创建ActionSheet对象
var actionSheet = new ActionSheet ();
设置按钮，默认包含取消按钮
actionSheet.Other_Button_Title = new List<string> (){ "按钮1", "按钮2" };
继承ActionSheet.IActionSheetListener，调用SetActionSheetListener，设置点击监听
actionSheet.SetActionSheetListener (this);
显示
actionSheet.Show (SupportFragmentManager);
