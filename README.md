# Algeria Geography Data Explorer

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

A structured pipeline for collecting, cleaning, and organizing Algeria's administrative geography data into machine-readable JSON formats. Ideal for developers, researchers, and data scientists working with Algerian regional data.

## Features

- **Web Scraping**: Automated extraction of Algerian wilaya (province) data from official sources
- **Bilingual Support**: Arabic and Latin script datasets
- **Standardized Output**: Clean JSON formats for easy integration
- **Reproducible Pipeline**: Clear documentation of data processing steps

## Table of Contents

- [Data Structure](#data-structure)
- [Contributing](#contributing)
- [Data Sources](#data-sources)
- [My Process Workflow](#process-workflow)
- [License](#license)
  

## Data Structure

1. **City Arabic Names ([wilayat_ar.json](wilayat_ar.json))**: 
   ```json
   [
     "ادرار",
     "الشلف",
     "الأغواط",
     "أم البواقي",
    "..."
   ]
   ```
2. **City Latin  Names ([wilayat_en.json](wilayat_en.json))**:
   ```json
    [
    "Adrar",
     "Chlef", 
    "Laghouat",
    "Oum El Bouaghi",
    "...."
    ]
  

## Contributing
**We welcome contributions through**:
- Issue reporting
- Pull requests
- Data validation
- Additional feature proposals
- Please follow standard GitHub workflows when contributing.


## Data Sources
 https://ar.wikipedia.org/wiki/%D9%88%D9%84%D8%A7%D9%8A%D8%A7%D8%AA_%D8%A7%D9%84%D8%AC%D8%B2%D8%A7%D8%A6%D8%B1



## Process Workflow
1- **Data Extraction**:

```python
  import pandas as pd
  tables = pd.read_html(source_url)
```
2- **Name Extraction**:

   - Arabic names from first column

  - Latin names from second column

3- **Data Cleaning**:

- Remove special characters

- Standardize naming conventions

- Validate against known administrative lists

4- **Export**:

- JSON serialization with UTF-8 encoding

- Pretty-printed formatting for readability


## License

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

This project is licensed under the **MIT License**.

### Key Permissions:
- ✅ Free to use for any purpose (personal, educational, commercial, ...)
- ✅ Freedom to modify and redistribute
- ✅ No liability or warranty provided


### Recommended Attribution:
While not legally required, we appreciate attribution through:
```bash
Data sourced from Algeria Geography Data Explorer (https://github.com/Ramzi-Hadrouk/Algeria-Geography-Data-Explorer)







