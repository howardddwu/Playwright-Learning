# **OrangeHRM Playwright Automation Project**

## **Overview**
This project automates testing for the OrangeHRM platform using [Playwright](https://playwright.dev/). It includes functional UI tests, API testing, and other test scenarios to ensure the platform's reliability and functionality.

---

## **Features**
- **UI Automation**: Test login, employee management, leave management, and performance modules.
- **API Testing**: Validate backend API endpoints for consistency with the UI.
- **Reusable Page Objects**: Encapsulated locators and actions for maintainable test scripts.
- **Data-Driven Testing**: Test scenarios with dynamic input data from JSON files.
- **Detailed Reports**: Generate HTML reports for test execution.

---

## **Tech Stack**
- **Language**: JavaScript/TypeScript  
- **Framework**: Playwright  
- **Testing Libraries**: Playwright Test  
- **Tools**: Node.js, dotenv (for environment variables)

---

## **Project Structure**
```plaintext
orangehrm-playwright-project/
│
├── tests/                          # Test files
│   ├── login/                      # Login module tests
│   ├── employee/                   # Employee management tests
│   ├── leave/                      # Leave management tests
│   └── performance/                # Performance review tests
│
├── pages/                          # Page Object Model files
├── fixtures/                       # Test data and fixtures
├── utils/                          # Utility functions
├── reports/                        # Test execution reports
│   ├── html-reports/               # HTML reports
│   └── logs/                       # Debugging logs
│
├── playwright.config.js            # Playwright configuration
├── package.json                    # Node.js dependencies
├── .env                            # Environment variables
├── README.md                       # Project documentation
└── .gitignore                      # Files to exclude from Git
```

## **Installation**
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/orangehrm-playwright-project.git](https://github.com/howardddwu/Playwright-Learning.git)
   cd orangehrm-playwright-project
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure environment variables:
   - Copy `.env.example` to `.env`
   - Update the variables with your OrangeHRM instance details:
   ```plaintext
   BASE_URL=https://your-orangehrm-instance.com
   ADMIN_USER=admin
   ADMIN_PASSWORD=your_password
   ```

## **Running Tests**
- Run all tests:
  ```bash
  npm test
  ```

- Run specific test file:
  ```bash
  npx playwright test tests/login/login.spec.ts
  ```

- Run tests in headed mode:
  ```bash
  npx playwright test --headed
  ```

- Run tests in specific browser:
  ```bash
  npx playwright test --project=chromium
  ```

## **Test Reports**
- HTML reports are automatically generated after test execution in `reports/html-reports`
- To view the latest report:
  ```bash
  npx playwright show-report
  ```

## **Writing Tests**
- Create new test files in the appropriate directory under `tests/`
- Use Page Objects from `pages/` directory
- Add test data in `fixtures/` directory
- Follow the existing patterns for consistency

## **Contributing**
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## **Best Practices**
- Keep tests independent and atomic
- Use meaningful descriptions for test cases
- Maintain page objects for better maintainability
- Use appropriate assertions
- Add comments for complex logic
- Follow the project's coding standards

## **Troubleshooting**
- Check the logs in `reports/logs/` for debugging information
- Ensure environment variables are correctly set
- Verify network connectivity to the OrangeHRM instance
- Check browser compatibility and versions

## **License**
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## **Contact**
Your Name - [@yourtwitter](https://twitter.com/yourtwitter)
Project Link: [https://github.com/yourusername/orangehrm-playwright-project](https://github.com/yourusername/orangehrm-playwright-project)
