# Exploratory Testing

## Session 01 – Templates and File Upload

**Objective:** Explore template creation and document upload functionality.

**Focus Areas:**

- Template creation
- File upload
- File replacement
- Input validation
- Long names
- Empty input
- Playbook generation

### Observations

During exploratory testing, the following behaviors were observed:

1. A document could be replaced by selecting another file.
2. After replacing a file, the stored file changed but the displayed filename remained unchanged.
3. Playbook generation returned an error after initiating the generation process.
4. Very long template names were accepted.
5. Template creation without a name was possible.

### Validation

Each observation was investigated further to determine whether it represented:

- Confirmed defect
- Expected behavior
- UX improvement
- Requirement clarification

Only validated defects were added to the Bug Reports directory.
