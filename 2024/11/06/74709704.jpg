<?php
// show_wifi.php

// 执行nmcli命令来列出所有可搜索到的WiFi网络
$output = shell_exec("nmcli -f SSID,BSSID,MODE,SIGNAL,SECURITY device wifi list 2>&1");

// 检查是否有错误或输出是否为空
if (empty(trim($output))) {
    echo "<p>没有找到任何WiFi网络。</p>";
} else {
    // 直接输出原始命令输出，并设置字号为22px
    echo "<pre style='font-size: 22px;'>$output</pre>";
}
?>