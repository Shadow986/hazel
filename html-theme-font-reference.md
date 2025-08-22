# HTML Theme and Font Reference

## CSS Variables for Theme Management

```css
:root {
  /* Light Theme Colors */
  --primary-color: #3b82f6;
  --secondary-color: #64748b;
  --background-color: #ffffff;
  --surface-color: #f8fafc;
  --text-primary: #1e293b;
  --text-secondary: #64748b;
  --border-color: #e2e8f0;
  --shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1);
  
  /* Dark Theme Colors */
  --dark-primary: #60a5fa;
  --dark-secondary: #94a3b8;
  --dark-background: #0f172a;
  --dark-surface: #1e293b;
  --dark-text-primary: #f1f5f9;
  --dark-text-secondary: #cbd5e1;
  --dark-border: #334155;
  --dark-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.3);
}
```

## Font Stack Examples

```css
/* System Font Stack */
.system-font {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen', 
               'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue', 
               sans-serif;
}

/* Google Fonts Examples */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap');

.inter-font { font-family: 'Inter', sans-serif; }
.poppins-font { font-family: 'Poppins', sans-serif; }
.roboto-font { font-family: 'Roboto', sans-serif; }

/* Monospace for Code */
.code-font {
  font-family: 'Fira Code', 'JetBrains Mono', 'SF Mono', Monaco, 'Cascadia Code', 
               'Roboto Mono', Consolas, 'Courier New', monospace;
}
```

## Complete HTML Template with Theme Support

```html
<!DOCTYPE html>
<html lang="en" data-theme="light">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Theme Reference</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
          /* Light Theme */
          --primary: #3b82f6;
          --secondary: #64748b;
          --background: #ffffff;
          --surface: #f8fafc;
          --text-primary: #1e293b;
          --text-secondary: #64748b;
          --border: #e2e8f0;
          --shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1);
        }

        [data-theme="dark"] {
          --primary: #60a5fa;
          --secondary: #94a3b8;
          --background: #0f172a;
          --surface: #1e293b;
          --text-primary: #f1f5f9;
          --text-secondary: #cbd5e1;
          --border: #334155;
          --shadow: 0 1px 3px 0 rgb(0 0 0 / 0.3);
        }

        * {
          margin: 0;
          padding: 0;
          box-sizing: border-box;
        }

        body {
          font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
          background-color: var(--background);
          color: var(--text-primary);
          line-height: 1.6;
          transition: background-color 0.3s ease, color 0.3s ease;
        }

        .container {
          max-width: 1200px;
          margin: 0 auto;
          padding: 2rem;
        }

        .card {
          background: var(--surface);
          border: 1px solid var(--border);
          border-radius: 8px;
          padding: 1.5rem;
          margin-bottom: 1rem;
          box-shadow: var(--shadow);
        }

        .btn {
          background: var(--primary);
          color: white;
          border: none;
          padding: 0.75rem 1.5rem;
          border-radius: 6px;
          cursor: pointer;
          font-weight: 500;
          transition: all 0.2s ease;
        }

        .btn:hover {
          opacity: 0.9;
          transform: translateY(-1px);
        }

        .theme-toggle {
          position: fixed;
          top: 1rem;
          right: 1rem;
          background: var(--surface);
          border: 1px solid var(--border);
          color: var(--text-primary);
        }

        h1, h2, h3 { 
          color: var(--text-primary);
          margin-bottom: 1rem;
        }

        p { 
          color: var(--text-secondary);
          margin-bottom: 1rem;
        }

        code {
          background: var(--surface);
          padding: 0.25rem 0.5rem;
          border-radius: 4px;
          font-family: 'Fira Code', monospace;
          border: 1px solid var(--border);
        }
    </style>
</head>
<body>
    <button class="btn theme-toggle" onclick="toggleTheme()">🌙</button>
    
    <div class="container">
        <div class="card">
            <h1>Theme Reference Page</h1>
            <p>This page demonstrates the theme system with CSS variables.</p>
            <button class="btn">Primary Button</button>
        </div>

        <div class="card">
            <h2>Typography Examples</h2>
            <h3>Heading 3</h3>
            <p>This is a paragraph with <code>inline code</code> styling.</p>
        </div>
    </div>

    <script>
        function toggleTheme() {
            const html = document.documentElement;
            const currentTheme = html.getAttribute('data-theme');
            const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
            html.setAttribute('data-theme', newTheme);
            
            const toggle = document.querySelector('.theme-toggle');
            toggle.textContent = newTheme === 'dark' ? '☀️' : '🌙';
        }
    </script>
</body>
</html>
```

## Popular Color Palettes

```css
/* Tailwind CSS Inspired */
.tailwind-palette {
  --blue-500: #3b82f6;
  --gray-500: #6b7280;
  --green-500: #10b981;
  --red-500: #ef4444;
  --yellow-500: #f59e0b;
  --purple-500: #8b5cf6;
}

/* Material Design */
.material-palette {
  --primary: #1976d2;
  --secondary: #dc004e;
  --surface: #ffffff;
  --background: #fafafa;
  --error: #b00020;
}

/* GitHub Dark */
.github-dark {
  --bg-primary: #0d1117;
  --bg-secondary: #161b22;
  --border: #30363d;
  --text-primary: #f0f6fc;
  --text-secondary: #8b949e;
  --accent: #58a6ff;
}
```

## Responsive Typography Scale

```css
.typography-scale {
  /* Mobile First */
  --text-xs: 0.75rem;    /* 12px */
  --text-sm: 0.875rem;   /* 14px */
  --text-base: 1rem;     /* 16px */
  --text-lg: 1.125rem;   /* 18px */
  --text-xl: 1.25rem;    /* 20px */
  --text-2xl: 1.5rem;    /* 24px */
  --text-3xl: 1.875rem;  /* 30px */
  --text-4xl: 2.25rem;   /* 36px */
}

@media (min-width: 768px) {
  .typography-scale {
    --text-3xl: 2.25rem;  /* 36px */
    --text-4xl: 3rem;     /* 48px */
  }
}
```

## Animation Utilities

```css
.fade-in {
  animation: fadeIn 0.3s ease-in-out;
}

.slide-up {
  animation: slideUp 0.4s ease-out;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes slideUp {
  from { 
    opacity: 0;
    transform: translateY(20px);
  }
  to { 
    opacity: 1;
    transform: translateY(0);
  }
}
```

## Usage Notes

- Use CSS custom properties (variables) for consistent theming
- Implement `data-theme` attribute switching for dark/light modes
- Choose font stacks that provide good fallbacks
- Test color contrast ratios for accessibility
- Use relative units (rem, em) for scalable typography
- Implement smooth transitions for theme changes
