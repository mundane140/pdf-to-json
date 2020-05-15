# pdf-to-json

## The idea

Put all the PDF books in the `sources` directory. Put all the templates (how you want to parse the book) in the `templates` directory. 
Assign templates to sources via a `config.yaml` file.
Here is a sample

```
- op1: 
  input: name_of_source.pdf
  template: name_of_template
  output: name_of_output.json
- op2: 
  input: name_of_source.pdf
  template: name_of_template
  output: name_of_output.json
```
Here `op1` and `op2` are used as log tags. For example, any logs for operation `op1` will start with the handle `OP1`. It is automatically converted to uppercase.
The json files with the name same as mentioned in the config file will be created after successful completion of operation in the `results` directory.
