# FORM SNIPPET

`form-snippet` is a React package that provides a simple and flexible way to handle forms with custom components.

## Table of Contents 📚

- [Badges](#badges)
- [Installation](#installation)
- [Usage/Examples](#usageexamples)
- [Contributing](#contributing)
- [📞 Contact Information](#-contact-information)
- [License](#license)

## Badges

| [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/) | [![form-snippet](https://img.shields.io/npm/v/form-snippet.svg)](https://www.npmjs.com/package/form-snippet) | ![NPM Downloads](https://img.shields.io/npm/dm/form-snippet) | ![npm bundle size](https://img.shields.io/bundlephobia/min/form-snippet) |
| -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------------------ |

## Installation

Install form-snippet with npm

```bash
  npm install form-snippet
```

Install form-snippet with github packages

```bash
  npm install @git21221/form-snippet@latest
```

## Usage/Examples

#### A signup form using form-snippet, took less than 50 lines of code and proper validation.

```javascript
import React from "react";
import {
  Button,
  Input,
  FormWrapper,
  SelectInput,
} from "@git21221/form-snippet";
import { months, dates, years, skills } from "./data/data";

function App() {
  const handleSubmit = (data) => {
    console.log(data);
  };

  return (
    <FormWrapper onSubmit={handleSubmit}>
      <div className="max-w-[400px] p-3 flex flex-col gap-3 shadow-2xl rounded-lg">
        <h1 className="text-xl">Signup using form-snippet</h1>
        <div className="flex gap-3">
          <Input
            name="fName"
            label="First Name"
            required
            type={"text"}
            fullWidth
          />
          <Input
            name="lName"
            label="Last Name"
            required
            type={"text"}
            fullWidth
          />
        </div>
        <div className="">
          <Input
            name="pass"
            label="Password"
            type="password"
            fullWidth
            endIcon
          />
        </div>
        <div className="">
          <Input
            name="mobile"
            label="Mobile number or email"
            type={"text"}
            fullWidth
          />
        </div>
        <div className="flex gap-3">
          <SelectInput
            name="month"
            label="Month"
            options={months}
            required
            fullWidth
          />
          <SelectInput
            name="date"
            label="Date"
            options={dates}
            required
            fullWidth
          />
          <SelectInput
            name="year"
            label="Year"
            options={years}
            required
            fullWidth
          />
        </div>
        <div>
          <SelectInput
            name="skills"
            label="Skills"
            options={skills}
            fullWidth
            multiple={{ checkBox: true }}
            renderStyle={"chip"}
          />
        </div>
        <Button content={"Submit"} />
      </div>
    </FormWrapper>
  );
}

export default App;
```

## Contributing

Contributions are always welcome!

See [contributing.md](./CONTRIBUTING.md) for ways to get started.

Please adhere to this project's [code of conduct](./CODE_OF_CONDUCT.md).

## 📞 **Contact Information**

### Project Admin⚡

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/Git21221/">
        <img src="https://avatars.githubusercontent.com/u/101005577?v=4" width="150px" height="150px" />
      </a>
      <br>
      <h4 style="color:red;">SAIKAT DAS</h4>
      <a href="https://www.linkedin.com/in/saikat-das-794711243/">
        <img src="https://img.icons8.com/fluency/2x/linkedin.png" width="32px" height="32px" />
      </a>
    </td>
  </tr>
</table>

Got questions? Want to suggest improvements? Open an issue on GitHub or contact the project admin, **Saikat Das**, at:  
📧 **saikatdas40g@gmail.com**



## License

[MIT](https://choosealicense.com/licenses/mit/)



