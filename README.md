### clipboard 复制到粘贴板功能
> 非常简单，只有一个copy功能。
```javascript
// 第一步，引入 copy-clipboard
<script src="copy-clipboard.js"></script>
or 
import "copy-clipboard.js"
// 第二步，复制功能 （注意，不能直接调用new CopyClipBoard， 会失败，需要用户与页面交互的情况下调用，比如点击事件发生时）
let copyBtn = document.getElementById('copyBtn');
copyBtn.onclick = function() {
  new CopyClipBoard('任何你想复制到粘贴板的值');
}
// now you are success 
```