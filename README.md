<div id="top"></div>
[![MIT License][license-shield]][license-url]

<br />

# Objects Merge

A javascript library used to merge multiple objects.

<br />

### Installation
---

NPM package
```sh
npm install objects-merge
```

### Usage
---

If you want to merge multiple objects
```sh
import { merge } from 'objects-merge';

const DefaultTheme = {
	Colors: {
		Black : "#000",
		White: "#FFF",	
	},
	textSize: {
        size: {
            body: "14px",
            paragraph: "14px",            
        },
        height: {
            body: "24px",
            paragraph: "26px",
            
        }
    }
};

const NewTheme = {
	Colors: {
		Gray: "#FAFBFB",
		Success: "#FAFDFC",
		Warning: "#FFFDF8",
		Disabled: "#B0B7C3",
	},
	textSize: {
        size: {
            title: "22px",
            heading: "26px",
        },
        height: {
            title: "32px",
            heading: "40px",
        }
    }
} 

let newMergedObject = merge(DefaultTheme, NewTheme);
```

### License
---
Distributed under the [MIT License](https://opensource.org/licenses/MIT)

[license-shield]: https://img.shields.io/badge/license-MIT-green
[license-url]: https://opensource.org/licenses/MIT