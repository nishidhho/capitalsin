# Contributing to Capital Sin

Thank you for your interest in Capital Sin! This is a **private personal project**, but these guidelines help maintain code quality and consistency.

## Code of Conduct

- Keep modifications **local and personal**
- Respect TogetherChat's terms of service
- Maintain **privacy** as a core principle
- No unauthorized distribution or modification for public use

---

## How to Contribute (Locally)

### **Reporting Issues**

If you find a bug or have a feature request:

1. Check existing issues first
2. Create a detailed issue with:
   - Steps to reproduce
   - Expected behavior
   - Actual behavior
   - Screenshots (if applicable)

### **Submitting Changes**

1. **Fork the repo** (if needed)
2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes**
4. **Test thoroughly**
5. **Commit with clear messages**
   ```bash
   git commit -m "feat: add your feature description"
   ```
6. **Push to your branch**
   ```bash
   git push origin feature/your-feature-name
   ```
7. **Submit a pull request** with a clear description

---

## Commit Message Convention

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <subject>

<body>

<footer>
```

### **Types:**
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation update
- `style`: Code style (formatting, missing semicolons, etc.)
- `refactor`: Code refactoring
- `perf`: Performance improvement
- `test`: Adding/updating tests
- `chore`: Build, dependencies, etc.

### **Examples:**
```
feat(gemini): add custom prompt support
fix(notion): handle missing token error
docs: update installation instructions
```

---

## Code Style

### **JavaScript**
- Use ES6+ syntax
- 2-space indentation
- Semicolons required
- Use meaningful variable names
- Add comments for complex logic

### **HTML/CSS**
- 2-space indentation
- Semantic HTML elements
- CSS class naming: `kebab-case`
- Mobile-first responsive design

### **File Organization**
```
capitalsin/
├── Core Files
│   ├── manifest.json
│   ├── background.js
│   ├── content.js
│   └── popup.html
├── Styling
│   └── style.css
├── Logic & Integration
│   ├── popup.js
│   └── notion_api.js
├── Assets
│   ├── icons/
│   └── libs/
└── Documentation
    └── README.md
```

---

## Testing

Before submitting changes:

1. **Test in Chrome DevTools**
   - Open DevTools: `F12` or `Ctrl+Shift+I`
   - Check console for errors
   - Test all export formats

2. **Test on TogetherChat**
   - Load unpacked extension
   - Have a test conversation
   - Try each export option

3. **Notion Integration**
   - Test with valid token
   - Verify page creation
   - Check formatting

4. **Gemini Integration** (if modified)
   - Test with valid API key
   - Try all task types
   - Verify output quality

---

## Development Workflow

### **Local Setup**
```bash
git clone https://github.com/nishidhho/capitalsin.git
cd capitalsin
# Load as unpacked extension in Chrome
```

### **Making Changes**
```bash
git checkout -b feature/my-feature
# Edit files...
git add .
git commit -m "feat(feature): description"
git push origin feature/my-feature
```

### **Pull Request Process**
1. Describe what changed and why
2. Link any related issues
3. Provide testing steps
4. Include before/after screenshots (if UI changes)

---

## Documentation

- Update **README.md** if you add/change features
- Add code comments for non-obvious logic
- Update **CHANGELOG.md** with version changes
- Keep **API documentation** current

---

## Performance Considerations

- Minimize DOM queries (cache selectors)
- Use efficient event listeners
- Lazy-load external dependencies
- Keep memory usage low (important for browser extensions)

---

## Security & Privacy

- **Never store API keys** in code
- Keep user data **local** by default
- Only send to external APIs when **explicitly requested**
- Validate all user inputs
- Clear sensitive data from memory

---

## Questions?

- Check the **README.md** for usage
- Review existing code for patterns
- Refer to Chrome Extension documentation
- Check Notion API docs for integration questions

---

## License

By contributing, you agree that your contributions will be licensed under the **MIT License**.

---

**Happy coding! 🚀**
