“真机远程调试”（remote inspect web on real device），是指用桌面电脑（PC或MAC）远程连接上移动设备，通过类似Chrome浏览器开发人员工具的界面，来调试移动设备上运行的网页

1.Chorme模拟器

在PC或MAC上打开Chrome浏览器，打开想要调试的页面，然后打开开发人员工具
点击开发人员工具顶栏上的手机图标，即可开始调试，一般来说需要重新刷新页面
在页面顶部可以看到设备选择下拉菜单 Device 和 模拟网络环境的下拉菜单 Network ，及左侧的清除选择按钮和打开关闭 media queries 的按钮
打开设置左边的那个类似 >三 的图标，切换到 Emulation 标签，可以更细粒度地调整，来定制化你的模拟

2.调试Android上的Chrome

在Android设备上安装Chrome浏览器（版本>=32，https://play.google.com/store/apps/details?id=com.android.chrome&hl=en ）（只有安卓4.0以上才有Chrome）
开启当前Android设备的USB调试
在PC或MAC上安装chrome浏览器（版本>=32）和对应的Android设备驱动（如果找不到，可以在这个 列表 内尝试）
用USB线连接Android设备，在PC或MAC上的chrome地址栏输入 chrome://inspect 然后回车，或通过菜单图标→工具→检查设备，进入调试界面
勾选界面中的 Discover USB devices ，直到搜索到你的Android设备
在移动设备上弹出的是否允许远程调试上，选择“允许”
在下面的页面列表（将展示已在Android上的chrome中打开的页面），点击对应的 inspect 开始调试
此时将在桌面版Chrome上弹出一个新的标签页，即为调试界面；如果很久都没用响应，请翻墙后再试（ 一个免费的梯子服务 ）（ 免费10天稳定梯子服务 ）
其他参考链接

https://developer.chrome.com/devtools/docs/remote-debugging

3.调试Android APP里的webview

通过修改代码，在APP内设置允许远程调试（需安卓版本为4.4及以上）： 方法 ，然后安装APP
开启当前Android设备的USB调试
在PC或MAC上安装chrome浏览器（版本>=32）和对应的Android设备驱动（如果找不到，可以在这个 列表 内尝试）
用USB线连接Android设备，在PC或MAC上的chrome地址栏输入 chrome://inspect 然后回车，或通过菜单图标→工具→检查设备，进入调试界面
勾选界面中的 Discover USB devices ，直到搜索到你的Android设备
在移动设备上弹出的是否允许远程调试上，选择“允许”
在下面的页面列表（将展示已在Android上的chrome中打开的页面），点击对应的 inspect 开始调试
此时将在桌面版Chrome上弹出一个新的标签页，即为调试界面；如果很久都没用响应，请翻墙后再试（ 一个免费的翻墙服务 ）
其他参考链接

https://developers.google.com/chrome-developer-tools/docs/remote-debugging


4.调试iOS上的Safari

在iOS设备上打开允许调试：设置→Safari→高级→打开”web检查器“
在MAC上打开Safari的开发菜单：顶部菜单栏“Safari”→偏好设置→高级→打开”在菜单栏中显示“开发”菜单
在iOS设备上的Safari浏览器中打开要调试的页面，然后切换到MAC的Safari，在顶部菜单栏选择“开发”→找到你的iOS设备名称→右边二级菜单选择需要调试的对应标签页，即可开始远程调试
如果没有iOS设备，也可以在Xcode中模拟一台，点击顶部“Xcode”→“Open Developer Tool”→“iOS Simulator”即可打开一个iOS设备的模拟器，并且模拟器里面Safari打开的页面，也是能通过上个步骤中MAC上的Safari调试。 