# Contributing to Nourivex Laravel Template

Thank you for your interest in contributing to the **Nourivex Laravel Template**! This template provides a modern, structured foundation for building robust and scalable Laravel web applications.

Contributions of all kinds are welcome—from bug fixes and documentation enhancements to developer experience improvements.

---

## 🛠️ Development Setup

### Prerequisites
- **PHP 8.3+**
- **Composer 2.x**
- **Node.js 22+ & npm**
- *(Recommended)* **DDEV** for isolated local container environments

### Getting Started

1. **Fork and Clone:**
   ```bash
   git clone https://github.com/Nourivex/nourivex-laravel-template.git
   cd nourivex-laravel-template
   ```

2. **Setup with DDEV (Recommended):**
   ```bash
   ddev start
   ddev composer setup
   ```

3. **Or Native Local Setup:**
   ```bash
   composer install
   cp .env.example .env
   php artisan key:generate
   php artisan migrate
   npm install
   npm run build
   ```

---

## 📋 Contribution Workflow

1. **Create a Topic Branch:**
   Always branch from `main`:
   ```bash
   git checkout -b feat/your-feature-name
   # or
   git checkout -b fix/your-bugfix-name
   ```

2. **Coding Standards:**
   We adhere to Laravel's coding standards. Format your code using **Laravel Pint** before submitting:
   ```bash
   ./vendor/bin/pint
   # Or with DDEV:
   ddev exec ./vendor/bin/pint
   ```

3. **Run Tests:**
   Ensure all existing and new tests pass:
   ```bash
   php artisan test
   ```

4. **Commit Conventions:**
   We follow [Conventional Commits](https://www.conventionalcommits.org/):
   - `feat:` for new features or capabilities
   - `fix:` for bug fixes
   - `docs:` for documentation updates
   - `refactor:` for code restructuring without changing behavior
   - `test:` for adding or updating tests

5. **Submit a Pull Request:**
   - Push your branch to your fork or origin:
     ```bash
     git push -u origin feat/your-feature-name
     ```
   - Open a Pull Request targeting the `main` branch.
   - Describe the changes made and link any related issues.

---

## 📄 License

By contributing to this repository, you agree that your contributions will be licensed under the project's [MIT License](LICENSE).
