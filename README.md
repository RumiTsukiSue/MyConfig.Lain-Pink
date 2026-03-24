# MyConfig.Lain-Pink
使用AI设计的Lain-Pink主题，对壁纸取色的反复修改，并参考了dracula

## base16
```
base00 = "121215";
base01 = "1A1A1D";
base02 = "4D4F60";
base03 = "626473";
base04 = "9A9AAD";
base05 = "E0E0D8";
base06 = "F0F0E8";
base07 = "FCFCF8";
base08 = "FF5555";
base09 = "FFB86C";
base0A = "FFF08C";
base0B = "7BC98D";
base0C = "8BE9FD";
base0D = "FF8888";
base0E = "FF79C6";
base0F = "BD93F9";
```

## noctalia配置
亮色模式是对dracula的直接复制
```
{
  "dark": {
    "mPrimary": "#FF8888",
    "mOnPrimary": "#121215",
    "mSecondary": "#FF79C6",
    "mOnSecondary": "#121215",
    "mTertiary": "#8BE9FD",
    "mOnTertiary": "#121215",
    "mError": "#FF5555",
    "mOnError": "#121215",
    "mSurface": "#121215",
    "mOnSurface": "#E0E0D8",
    "mSurfaceVariant": "#1A1A1D",
    "mOnSurfaceVariant": "#9A9AAD",
    "mOutline": "#4D4F60",
    "mShadow": "#121215",
    "mHover": "#4D4F60",
    "mOnHover": "#E0E0D8",
    "terminal": {
      "normal": {
        "black": "#121215",
        "red": "#FF5555",
        "green": "#7BC98D",
        "yellow": "#FFF08C",
        "blue": "#FF8888",
        "magenta": "#FF79C6",
        "cyan": "#8BE9FD",
        "white": "#E0E0D8"
      },
      "bright": {
        "black": "#626473",
        "red": "#FF5555",
        "green": "#7BC98D",
        "yellow": "#FFF08C",
        "blue": "#FF8888",
        "magenta": "#FF79C6",
        "cyan": "#8BE9FD",
        "white": "#FCFCF8"
      },
      "foreground": "#E0E0D8",
      "background": "#121215",
      "selectionFg": "#E0E0D8",
      "selectionBg": "#4D4F60",
      "cursorText": "#121215",
      "cursor": "#E0E0D8"
    }
  },
  "light": {
    "mPrimary": "#d7827e",
    "mOnPrimary": "#faf4ed",
    "mSecondary": "#56949f",
    "mOnSecondary": "#faf4ed",
    "mTertiary": "#286983",
    "mOnTertiary": "#faf4ed",
    "mError": "#b4637a",
    "mOnError": "#faf4ed",
    "mSurface": "#fffaf3",
    "mOnSurface": "#575279",
    "mSurfaceVariant": "#f2e9e1",
    "mOnSurfaceVariant": "#797593",
    "mOutline": "#dfdad9",
    "mShadow": "#faf4ed",
    "mHover": "#cecacd",
    "mOnHover": "#575279",
    "terminal": {
      "normal": {
        "black": "#f2e9e1",
        "red": "#b4637a",
        "green": "#286983",
        "yellow": "#ea9d34",
        "blue": "#56949f",
        "magenta": "#907aa9",
        "cyan": "#d7827e",
        "white": "#575279"
      },
      "bright": {
        "black": "#9893a5",
        "red": "#b4637a",
        "green": "#286983",
        "yellow": "#ea9d34",
        "blue": "#56949f",
        "magenta": "#907aa9",
        "cyan": "#d7827e",
        "white": "#575279"
      },
      "foreground": "#575279",
      "background": "#faf4ed",
      "selectionFg": "#575279",
      "selectionBg": "#dfdad9",
      "cursorText": "#faf4ed",
      "cursor": "#575279"
    }
  }
}
```

## nvim配置
```
-- 基础 UI
hl("Normal", { fg = c.base05, bg = c.base00 })
hl("CursorLine", { bg = c.base01 })
hl("LineNr", { fg = c.base03 })
hl("CursorLineNr", { fg = c.base0D, bold = true })
hl("Visual", { bg = c.base02 })
hl("Search", { bg = c.base0A, fg = c.base00 })
hl("IncSearch", { bg = c.base09, fg = c.base00 })
hl("StatusLine", { fg = c.base04, bg = c.base02 })
hl("VertSplit", { fg = c.base02, bg = c.base00 })
hl("ColorColumn", { bg = c.base01 })

-- 语法基础
hl("Comment", { fg = c.base03, italic = true })
hl("String", { fg = c.base0B })
hl("Number", { fg = c.base09 })
hl("Keyword", { fg = c.base0E, bold = true })
hl("Function", { fg = c.base0D })
hl("Statement", { fg = c.base0E })
hl("Type", { fg = c.base0A })
hl("Identifier", { fg = c.base08 })
hl("Special", { fg = c.base0C })

-- Treesitter 映射
hl("@variable", { fg = c.base05 })
hl("@function", { fg = c.base0D })
hl("@keyword", { fg = c.base0E, bold = true })
hl("@property", { fg = c.base08 })
hl("@type", { fg = c.base0A })
hl("@string", { fg = c.base0B })
hl("@constant", { fg = c.base09 })
hl("@parameter", { fg = c.base08 })

-- LSP 诊断颜色
hl("DiagnosticError", { fg = c.base08 })
hl("DiagnosticWarn", { fg = c.base0A })
hl("DiagnosticInfo", { fg = c.base0D })
hl("DiagnosticHint", { fg = c.base0C })

-- 补全菜单 (Pmenu)
hl("Pmenu", { bg = c.base01, fg = c.base05 })
hl("PmenuSel", { bg = c.base0D, fg = c.base00 })

-- 侧边栏/文件树高亮
hl("NvimTreeNormal", { bg = c.base01, fg = c.base05 })
hl("NvimTreeEndOfBuffer", { fg = c.base01 })
```
