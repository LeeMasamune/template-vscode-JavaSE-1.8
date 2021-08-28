# template-vscode-JavaSE-1.8

*Template for JavaSE-1.8 development in vscode*

May work for other Java versions by editing some of the files described below.

## Extensions

Tested on:
- redhat.java v0.81.0
- vscjava.vscode-java-dependency v0.18.7

## Project files

`${workspaceFolder}/.settings/org.eclipse.jdt.core.prefs`
```properties
org.eclipse.jdt.core.compiler.codegen.targetPlatform=1.8
org.eclipse.jdt.core.compiler.source=1.8
```

`${workspaceFolder}/.classpath`
```xml
<?xml version="1.0" encoding="UTF-8"?>
<classpath>
	<classpathentry kind="con" path="org.eclipse.jdt.launching.JRE_CONTAINER/org.eclipse.jdt.internal.debug.ui.launcher.StandardVMType/JavaSE-1.8"/>
	<classpathentry kind="src" path="src"/>
	<classpathentry kind="output" path="bin"/>
</classpath>
```

`${workspaceFolder}/.project`
```xml
<?xml version="1.0" encoding="UTF-8"?>
<projectDescription>
	<name>YOUR_PROJECT_NAME</name>
	<comment></comment>
	<projects>
	</projects>
	<buildSpec>
		<buildCommand>
			<name>org.eclipse.jdt.core.javabuilder</name>
			<arguments>
			</arguments>
		</buildCommand>
	</buildSpec>
	<natures>
		<nature>org.eclipse.jdt.core.javanature</nature>
	</natures>
	<filteredResources>
	</filteredResources>
</projectDescription>
```

## Working with Eclipse

It's better to have Eclispe to generate these the above project files.
To have Java extensions detect the correct JRE System Library, in Eclipse set
the execution environment JRE or the project specific JRE to a name defined in
user setting `java.configuration.runtimes`.


## License

[Unlicense](LICENSE).
