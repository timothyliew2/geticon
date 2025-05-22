# Icon Fetcher 设计规范文档

## 🎨 配色方案

### 主要颜色
- 主色：`--primary-color: #3b82f6`
- 主色悬停：`--primary-hover: #2563eb`
- 背景色：`#ffffff`
- 卡片背景：`--card-background: #ffffff`

### 辅助颜色
- 次要色：`--secondary-color: #64748b`
- 次要悬停：`--secondary-hover: #475569`
- 成功色：`--success-color: #22c55e`
- 错误色：`--error-color: #ef4444`

### 文字颜色
- 主要文字：`--text-color: #1e293b`
- 次要文字：`--text-secondary: #64748b`
- 边框颜色：`--border-color: #e2e8f0`

## 🔲 阴影与圆角

### 阴影
- 小阴影：`--shadow-sm: 0 1px 3px rgba(0,0,0,0.1)`
- 中阴影：`--shadow-md: 0 4px 6px -1px rgba(0,0,0,0.1)`
- 大阴影：`--shadow-lg: 0 10px 15px -3px rgba(0,0,0,0.1)`

### 圆角
- 小圆角：`--radius-sm: 0.375rem`
- 中圆角：`--radius-md: 0.5rem`
- 大圆角：`--radius-lg: 1rem`

## 🔘 按钮样式

### 语言切换按钮
```css
display: flex
align-items: center
gap: 6px
border: none
padding: 8px 16px
border-radius: 20px
background: var(--primary-color)
color: white
```

### 社区按钮
```css
display: flex
align-items: center
gap: 6px
border: none
padding: 8px 16px
border-radius: 20px
```

## 📦 容器样式

### 主容器
```css
width: 100%
padding: 2rem
margin: 0
```

### 模态框
```css
position: relative
background: var(--card-background)
margin: 15% auto
padding: 0
width: 90%
max-width: 400px
border-radius: 12px
box-shadow: var(--shadow-lg)
```

## 💫 动画效果

### 过渡动画
- 全局过渡：`--transition: all 0.3s ease`

### 淡入动画
```css
@keyframes fadeIn {
    from { opacity: 0; transform: translateY(-10px); }
    to { opacity: 1; transform: translateY(0); }
}
```

### 上滑动画
```css
@keyframes slideUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}
```

## 📱 响应式设计

### 移动端适配
```css
@media (max-width: 640px) {
    .app-results {
        grid-template-columns: repeat(auto-fill, minmax(200px, 1fr))
        gap: 1rem
        padding: 0.5rem
    }
}
```

## 🎯 设计原则

1. **简洁性**
   - 白色背景突出内容
   - 清晰的视觉层级
   - 适当的留白空间

2. **交互性**
   - 平滑的过渡动画
   - 清晰的状态反馈
   - 直观的操作方式

3. **一致性**
   - 统一的颜色系统
   - 一致的间距规范
   - 统一的交互模式

## 🔍 注意事项

1. 保持背景纯白，突出内容
2. 使用合适的间距和留白
3. 确保交互反馈的及时性
4. 保持移动端的良好体验
5. 注意文字的可读性和对比度
