# MMEETT 品牌颜色应用指南

## ✅ 已完成的 CSS 颜色更新

### 核心颜色板
```css
Coral Red (主色):  #FF6B6B - CTA 按钮、主要按钮、关键高亮
Cyan (强调色):     #00D4FF - 图标、次要高亮、链接
Purple (辅助色):   #8B5CF6 - 次要按钮、边框、装饰
Navy (深色背景):   #0A1628 - 主背景、深色区域、页脚
Navy Light:        #1a2840 - 卡片背景
Light Gray:        #F5F7FA - 区域分隔、微妙背景
```

### 已更新的 CSS 类

#### 1. **工具类颜色**
```css
.mmeett-coral { color: #FF6B6B; }
.mmeett-cyan { color: #00D4FF; }
.mmeett-purple { color: #8B5CF6; }
.mmeett-navy { color: #0A1628; }
.bg-mmeett-coral { background: #FF6B6B; }
.bg-mmeett-cyan { background: #00D4FF; }
.bg-mmeett-purple { background: #8B5CF6; }
.bg-mmeett-navy { background: #0A1628; }
.bg-mmeett-navy-light { background: #1a2840; }
.bg-section-light { background: #F5F7FA; }
```

#### 2. **渐变背景**
```css
.gradient-hero {
    background: linear-gradient(135deg, #0A1628 0%, #1a2840 100%);
}
.gradient-pricing {
    background: linear-gradient(180deg, #0A1628 0%, #1a2840 100%);
}
```

#### 3. **按钮样式**
```css
.cta-button {
    background: #FF6B6B;
    color: #FFFFFF;
}
.cta-button:hover {
    background: #ff5252;
}
```

#### 4. **区域样式**

**Hero 区域**
- 背景：海军蓝渐变 `#0A1628 → #1a2840`
- 标题：白色 `#FFFFFF`
- 副标题：白色 90% 透明度 `rgba(255,255,255,0.9)`

**Story 区域**
- 背景：浅灰 `#F5F7FA`
- 标题：海军蓝 `#0A1628`
- 正文：深灰 `#2D3748`

**Problem 区域**
- 背景：浅灰 `#F5F7FA`
- 标题：海军蓝 `#0A1628`
- 正文：深灰 `#2D3748`

**Transformation 区域**
- 背景：浅灰 `#F5F7FA`
- 时间线边框：紫色 `#8B5CF6`
- 强调文字：珊瑚红 `#FF6B6B`

**FAQ 区域**
- 背景：浅灰 `#F5F7FA`
- 标题：海军蓝 `#0A1628`
- 问题边框：紫色 `#8B5CF6`
- 问题悬停：珊瑚红 `#FF6B6B`
- 图标：青色 `#00D4FF`
- 答案：深灰 `#2D3748`

**Guarantee 区域**
- 背景：浅灰 `#F5F7FA`
- 边框：紫色 `#8B5CF6`
- 标题：海军蓝 `#0A1628`
- 正文：深灰 `#2D3748`

**Checkmarks 区域**
- 背景：浅灰 `#F5F7FA`
- 列表项边框：紫色 `#8B5CF6`
- 对勾图标：珊瑚红 `#FF6B6B`

**Pricing Card**
- 背景：海军蓝浅 `#1a2840`
- 边框：珊瑚红 `#FF6B6B` 3px
- 标题：白色 `#FFFFFF`
- 价格：珊瑚红 `#FF6B6B`
- 特性列表：白色 85% 透明度 `rgba(255,255,255,0.85)`
- 对勾：珊瑚红 `#FF6B6B`

**Tier Comparison**
- 背景：海军蓝渐变 `#0A1628 → #1a2840`
- 标题：白色 `#FFFFFF`
- 卡片背景：海军蓝浅 `#1a2840`
- 卡片边框（普通）：紫色 `#8B5CF6` 2px
- 卡片边框（推荐）：珊瑚红 `#FF6B6B` 3px
- 价格：珊瑚红 `#FF6B6B`
- CTA 按钮：珊瑚红 `#FF6B6B`

**MMEETT Features Section**
- 背景：海军蓝渐变 `#0A1628 → #1a2a4a`
- 标题：白色 `#FFFFFF`
- 卡片背景：半透明白色 `rgba(255,255,255,0.1)`
- 卡片边框：
  - AI 内容生成：珊瑚红 `#FF6B6B`
  - AI 名片：青色 `#00D4FF`
  - AI 翻译器：紫色 `#8B5CF6`
  - AI 会议助手：珊瑚红 `#FF6B6B`
  - 营销自动化：青色 `#00D4FF`

**Footer**
- 背景：海军蓝 `#0A1628`
- 顶部边框：珊瑚红 `#FF6B6B` 2px
- 文字：白色 70% 透明度 `rgba(255,255,255,0.7)`
- 链接：青色 `#00D4FF`，悬停：珊瑚红 `#FF6B6B`

---

## 📋 需要在 HTML 中手动更新的部分

### 1. Hero Section (已部分完成)
```html
<!-- 已应用 gradient-hero 类 -->
<section class="hero fade-up">
    <h1>从不懂 AI → 用 AI 赚钱</h1>
    <!-- 文字自动白色 -->
</section>
```

### 2. Story Section
```html
<!-- 添加 section-label -->
<section class="story slide-left">
    <div>
        <p style="color: #8B5CF6; font-size: 0.9rem; margin-bottom: 10px;">关于 Albert</p>
        <h2 style="color: #0A1628;">关于 Albert</h2>
        <!-- 高亮文字使用珊瑚红 -->
        <p>我是视频编辑师。<span style="color: #FF6B6B; font-weight: 700;">2 年经验</span>。</p>
    </div>
</section>
```

### 3. Quote Boxes (如果有)
```html
<div style="background: #0A1628; color: #FFFFFF; border-left: 4px solid #FF6B6B; padding: 20px;">
    引用内容
</div>
```

### 4. Links
```html
<a href="..." style="color: #00D4FF;">链接文字</a>
<!-- 悬停时变珊瑚红 -->
```

### 5. Section Labels
```html
<p style="color: #00D4FF; font-size: 0.9rem; margin-bottom: 10px;">MMEETT AI 平台功能</p>
<h2 style="color: #FFFFFF;">一站式 AI 解决方案</h2>
```

---

## 🎨 UI 元素颜色参考

| 元素 | 颜色 |
|------|------|
| **主要按钮** | `#FF6B6B` 背景，`#FFFFFF` 文字 |
| **次要按钮** | `#8B5CF6` 背景，`#FFFFFF` 文字 |
| **第三按钮** | 透明背景，`#FF6B6B` 边框，`#FF6B6B` 文字 |
| **链接（默认）** | `#00D4FF` (青色) |
| **链接（悬停）** | `#FF6B6B` (珊瑚红) |
| **区域分隔线** | `#8B5CF6` 1px 实线 (紫色) |
| **卡片边框** | `#8B5CF6` 2px 实线 (紫色) |
| **推荐卡片边框** | `#FF6B6B` 3px 实线 (珊瑚红) |
| **徽章背景** | `#FF6B6B` (珊瑚红) |
| **徽章文字** | `#FFFFFF` (白色) |
| **功能图标** | `#FF6B6B` (珊瑚红) |
| **装饰图标** | `#00D4FF` (青色) |
| **输入框** | `#1a2840` 背景，`#FFFFFF` 文字，`#8B5CF6` 边框 |
| **输入框聚焦** | `#00D4FF` 边框 (青色) |

---

## ✅ 已完成的项目

- [x] CSS 颜色变量定义
- [x] 渐变背景定义
- [x] CTA 按钮样式
- [x] Hero 区域背景渐变
- [x] Story 区域浅灰背景
- [x] Problem 区域浅灰背景
- [x] Transformation 区域浅灰背景
- [x] FAQ 区域浅灰背景 + 紫色边框
- [x] Guarantee 区域浅灰背景 + 紫色边框
- [x] Checkmarks 区域浅灰背景 + 紫色边框
- [x] Pricing Card 深蓝背景 + 珊瑚红边框
- [x] Tier Comparison 深蓝渐变背景
- [x] MMEETT Features 深蓝渐变背景
- [x] Footer 深蓝背景 + 珊瑚红顶部边框
- [x] 所有悬停效果（珊瑚红）
- [x] 进度条渐变（珊瑚红 → 青色）

---

## 📱 移动端优化（已包含）

```css
@media (max-width: 768px) {
    .container { padding: 15px; }
    .hero { padding: 60px 15px 40px; }
    .hero h1 { font-size: 2.2rem; }
    .cta-button { 
        width: 100%; 
        max-width: 320px;
        padding: 16px 35px;
    }
    /* 保持颜色不变 */
}
```

---

## 🚀 测试清单

### 桌面端测试
- [ ] Hero 区域渐变显示正确
- [ ] 所有 CTA 按钮为珊瑚红
- [ ] 悬停效果变为深珊瑚红
- [ ] FAQ 展开/折叠动画流畅
- [ ] 定价卡片边框颜色正确
- [ ] Footer 背景为深蓝

### 移动端测试
- [ ] 所有区域在小屏幕上显示正常
- [ ] 文字对比度足够
- [ ] CTA 按钮易于点击
- [ ] 卡片边框颜色清晰可见

---

## 💡 使用建议

1. **保持一致性**：所有相同类型的元素使用相同颜色
2. **对比度检查**：确保文字在背景上清晰可读
3. **悬停状态**：所有可点击元素都有悬停效果
4. **渐变使用**：仅在 Hero 和 Pricing 区域使用渐变
5. **白色空间**：浅灰背景区域保持足够留白

---

**更新日期：** 2026 年 4 月 13 日  
**状态：** ✅ CSS 颜色更新完成  
**下一步：** 在浏览器中预览效果
