# 华南理工大学计算机相关课程自动互评脚本（默认好评）

该油猴脚本用于华南理工大学计算机相关课程的自动互评，能够实现自动化操作，具体功能包括：
1. 自动选择评分（默认为 100 分）。
2. 自动填写评语（默认为“回答的很好，100分”）。
3. 自动切换学生作业和题目，直到所有任务评审完成。

## 功能说明

- **自动评分**：该脚本将自动为每个学生的作业评分，默认为 100 分。
- **自动填写评语**：评语自动设置为“回答的很好，100分”。
- **自动切换学生与题目**：在批改过程中，脚本会定时切换到下一个学生和作业题目，确保评审任务的连续性。

## 安装方法

1. 安装 **Tampermonkey** 或 **Greasemonkey** 插件：
   - [Tampermonkey 安装页面](https://www.tampermonkey.net/)
   - [Greasemonkey 安装页面](https://www.greasespot.net/)

2. 在 Tampermonkey 或 Greasemonkey 插件中添加新脚本。

3. 将脚本代码粘贴到新脚本中，保存并启用。

4. 打开目标网站 `http://1024.se.scut.edu.cn/`，脚本将在该网站上自动执行。

## 使用说明

- 脚本将在打开网站后自动运行，进行互评任务的自动化处理。
- 默认设置为自动评分为 100 分，评语为“回答的很好，100分”。
- 脚本每隔 15-16 秒执行一次，检查是否需要切换学生作业或题目，确保任务顺利进行。
- 可以用开发者工具（F12 → "Console"）在控制台看到脚本执行情况。输入以下命令可以来查看日志：

  ```javascript
  console.log(localStorage.getItem('script1_log')); 
  console.log(localStorage.getItem('script2_log')); 
  ```

  日志会持续累积，如果你想清除旧的日志，可以手动删除或在每次执行前清除。

  ```javascript
  localStorage.removeItem('script1_log'); 
  localStorage.removeItem('script2_log');

## 使用效果

![image](https://github.com/BAIKEMARK/Just_for_fun/blob/main/网页图.png)

![image](https://github.com/BAIKEMARK/Just_for_fun/blob/main/console_1.png)

![image](https://github.com/BAIKEMARK/Just_for_fun/blob/main/console_2.png)


## 注意事项

- 请确保在使用该脚本前已登录华南理工大学相关的在线作业平台。
- 如果脚本没有自动运行，尝试刷新页面或检查浏览器的 Tampermonkey 插件是否已启用。

## 许可证

该脚本使用 **GPL-3.0 许可证**，详见 [LICENSE](https://opensource.org/licenses/GPL-3.0)。

## 更新记录

### 版本 1.0
- 初始发布，支持自动评分、自动评语和切换学生作业。

## 联系方式

- 作者：BAIKEMARK
- 如有问题或建议，请在 GitHub 仓库中提交 Issue 或 Pull Request。
