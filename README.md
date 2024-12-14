# ng-universities

This is a public API of comprehensive, community-driven database of Nigerian universities, their faculties, and departments.

## How to Contribute

### Adding University Data

1. **Data Format**:
   - Create a new JSON file in the `data/universities/` directory
   - Name the file using the university's lowercase name with hyphens (e.g., `kwara-state-university.json`)
   - Follow the standard JSON structure provided in the documentation

2. **Contribution Steps**:
   - Fork the repository
   - Create a new branch (`git checkout -b add-university-data`)
   - Add your university JSON file
   - Run data validation script
   - Commit changes
   - Create a Pull Request

### Data Validation

Before submitting:
- Ensure all required fields are filled
- Validate JSON structure
- Check for accuracy of information

If you forget to do this. Do not fret, the CI workflow would help us detect it in your PR.

See below is an example structure we're looking for.

```json
{
  "name": "Full University Name",
  "acronym": "Acronym",
  "location": {
    "city": "City Name",
    "state": "State Name"
  },
  "founded": 1900,
  "website": "https://university.edu.ng",
  "faculties": [
    {
      "name": "Faculty Name",
      "departments": [
        "Department 1",
        "Department 2"
      ]
    }
  ]
}
```


## License
[MIT]
