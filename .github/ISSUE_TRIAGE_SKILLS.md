# ISSUE Triage Skills for `top.hookvip.pro`

> Repository: `Xposed-Modules-Repo/top.hookvip.pro`
>
> Purpose: Define the preferred workflow and rules for triaging GitHub issues in this repository so future issue handling can follow the same conventions without repeating instructions.

## 1. Core workflow

For **every category** of issues:

1. **List the issues first**
2. **Propose the handling plan**
   - whether to close
   - whether to reply
   - whether to modify title/body
   - what labels to add
   - what close reason to use
3. **Wait for confirmation**
4. **Execute only after confirmation**

Do **not** batch-handle a category without confirmation.

---

## 2. Comment convention

All automated assistant replies should begin with:

```text
[AI]
```

---

## 3. Default close behavior

Unless otherwise specified:

- add label: `已处理`
- close reason: `not_planned`

---

## 4. Title conventions

### 4.1 Bug / issue feedback

Use:

```text
【问题反馈】 xxx
```

### 4.2 Adaptation request

Use:

```text
【适配请求】 应用名称
```

### 4.3 Title editing rule

If an issue's **content is clear but the title is non-standard**, it may be renamed.

But before renaming:

1. list the affected issues
2. show current title and proposed new title
3. wait for confirmation
4. rename after confirmation

---

## 5. A 类：问题反馈缺材料 / 特殊原因

### A1. 明显乱填、敷衍填写

Handling:

- reply
- add `已处理`
- close

Recommended reply:

```text
[AI] 提交内容未按模板规范填写，关键信息无效，无法处理。请按模板完整填写问题描述、截图/视频及 LSPosed 日志后重新提交。
```

### A2. 反馈的是内测功能，公测版本没有

Handling:

- reply
- add `已处理`
- close

Recommended reply:

```text
[AI] 该功能为内测功能，公测版本暂无此功能。
```

### A3. 更像服务器侧问题

Handling:

- reply
- add `已处理`
- close

Recommended reply:

```text
[AI] 该问题更可能是服务器侧功能或服务端控制导致，暂不作为模块问题处理。
```

### A4. 边界问题先不动

Not all issues with missing logs/screenshots should be closed immediately.
Some should be left untouched and judged case by case.

---

## 6. B 类：广告相关 issue

These must be split into three groups first.

### B1. 纯“去广告”需求

Definition:

- only ad removal is requested
- no ad-reward bypass
- no other major function request

Handling:

- reply with AdClose guidance
- add `已处理`
- close

Recommended reply:

```text
[AI] 该需求属于去广告类需求，仓库模板已说明此类需求请使用 AdClose，故不在本仓库处理。
```

### B2. “免广告领奖励 / 看广告解锁权益”类

Definition:

- not simple ad removal
- user wants reward/time/benefit without watching ads

Handling:

- keep open for now
- do not process yet

### B3. “去广告 + 其他功能”混合类

Definition:

- ad removal is only one part
- also includes VIP unlock, root detection bypass, other feature unlocks, etc.

Handling:

- keep open for now
- do not process yet

---

## 7. C 类：字段填写错误 / issue 内容修正

### C1. 下载地址为空

Handling preference:

- can be ignored

### C2. 明显字段填错

Examples:

- app name filled with a download link
- invalid packer/protection status
- malformed markdown link
- download address filled with repository zip/tag asset instead of app link

Handling preference:

- may be corrected
- confirm before editing
- make the **smallest necessary change**
- usually no comment needed when silently correcting

### C3. If the issue is also duplicate

Priority rule:

- **duplicate handling takes precedence**
- do not spend time fixing the body if it will be closed as duplicate

---

## 8. D 类：重复 issue

Handling:

- keep the better submission
- close the duplicate(s)
- reply with the kept issue number/link
- remind the user not to submit duplicates
- add `已处理`

Recommended reply:

```text
[AI] 与已有 issue 重复，保留继续跟进：#xxx。请勿重复提交。
```

### Confirmed preferred kept issues in this repository

- Todo便签: keep `#413`
- 绿茶VPN: keep `#374`
- 零秒CarPlus: keep `#173`
- 长图拼接大师: keep `#325`
- 飞鸟听书: keep `#121`

---

## 9. 内容表述规则

### 9.1 内容表述不清

Definition:

- request is too vague
- cannot determine the actual requested functionality
- not actionable for maintainers

Handling:

- reply
- add `已处理`
- close

Recommended reply:

```text
[AI] 当前提交内容表述不清，无法判断具体诉求，暂不处理。请补充明确的功能需求后重新提交。
```

### 9.2 类型不符

Definition:

- issue was filed under the wrong template/category
- e.g. a bug report submitted as an adaptation request

Handling:

- reply
- add `已处理`
- close
- remind the user to use the proper template

Recommended reply:

```text
[AI] 该 issue 内容属于问题反馈/功能失效，不属于适配请求。请按“问题反馈”模板重新提交。
```

---

## 10. Preferred execution order

When asked to handle a category:

1. first list the matching open issues
2. then propose the handling plan
3. wait for confirmation
4. execute after confirmation

---

## 11. Reusable reply templates

### 11.1 去广告类

```text
[AI] 该需求属于去广告类需求，仓库模板已说明此类需求请使用 AdClose，故不在本仓库处理。
```

### 11.2 重复 issue

```text
[AI] 与已有 issue 重复，保留继续跟进：#xxx。请勿重复提交。
```

### 11.3 内容表述不清

```text
[AI] 当前提交内容表述不清，无法判断具体诉求，暂不处理。请补充明确的功能需求后重新提交。
```

### 11.4 类型不符

```text
[AI] 该 issue 内容属于问题反馈/功能失效，不属于适配请求。请按“问题反馈”模板重新提交。
```

### 11.5 明显乱填 / 敷衍填写

```text
[AI] 提交内容未按模板规范填写，关键信息无效，无法处理。请按模板完整填写问题描述、截图/视频及 LSPosed 日志后重新提交。
```

### 11.6 内测功能，公测无此功能

```text
[AI] 该功能为内测功能，公测版本暂无此功能。
```

### 11.7 可能是服务器功能

```text
[AI] 该问题更可能是服务器侧功能或服务端控制导致，暂不作为模块问题处理。
```

---

## 12. One-line summary

In `top.hookvip.pro`, issue triage should always be done category-by-category: list first, propose plan, wait for confirmation, then execute; use `[AI]` in comments; add `已处理` when closing unless told otherwise; close pure ad-removal requests with AdClose guidance; keep ad-reward and mixed requests for now; close unclear or miscategorized issues; and for duplicates, keep the better submission and close the rest.
