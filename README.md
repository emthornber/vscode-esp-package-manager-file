# esp-package-manager-file README

VS Code extension for colorizing ESP Package Manager definition files.

## Features

An EPM definition file has comments, directives, variables, file definitions, and HERE documents.
These are mapped to language scopes which are detailed below with examples :-

- Single Line Comment `comment.line` `#   24 November, 2023 - E M Thornber`
- Directive `entity.name.type` `%requires network-manager`
- Variable definition `variable.other` `$SCTL=/usr/bin/systemctl`
- Variable reference `variable.parameter` `${SCTL} daemon-reload`
- File definition `entity.name.type` `d 755 root root /usr -`
- HERE document `source.shell`
```
%postinstall <<EOF

${SCTL} daemon-reload
${SCTL} enable autowapctl

EOF
```

## Version history

### 0.1.0

- Initial release

