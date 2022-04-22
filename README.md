# COBOL Control Flow

COBOL Control Flow is an extension for Visual Studio Code that provides graphical visualization of program flow for programs written in COBOL. The extension is designed to help COBOL developers to quickly comprehend and debug COBOL programs with which they might not be familiar.

COBOL Control Flow displays paragraphs of a COBOL program as graphical nodes in an interactive graph. The edges of the graph are drawn based on the 'PERFORM' COBOL execution statements. You can interact with the graph to navigate to the relevant parts of the COBOL code, or you can navigate from the COBOL code to the relevant nodes in the graph.

COBOL Control Flow is part of [Code4z](https://marketplace.visualstudio.com/items?itemName=broadcomMFD.code4z-extension-pack), an all-round package that offers a modern experience for mainframe application developers, including [COBOL Langage Support](https://marketplace.visualstudio.com/items?itemName=broadcomMFD.cobol-language-support), [HLASM Language Support](https://marketplace.visualstudio.com/items?itemName=broadcomMFD.hlasm-language-support), [Explorer for Endevor](https://marketplace.visualstudio.com/items?itemName=broadcomMFD.explorer-for-endevor), [Zowe Explorer](https://marketplace.visualstudio.com/items?itemName=Zowe.vscode-extension-for-zowe) and [Debugger for Mainframe](https://marketplace.visualstudio.com/items?itemName=broadcomMFD.debugger-for-mainframe) extensions.

> **Note:** 
> - The COBOL Control Flow extension only supports IBM Enterprise COBOL. Other versions of COBOL are not supported.
> - We recommend you also install [COBOL Language Support](https://marketplace.visualstudio.com/items?itemName=broadcomMFD.COBOL-language-support) for COBOL code syntax awareness, to avoid generating COBOL Control Flow graphs from syntactically faulty code, and to enable copybook support features.

## Getting Started

### Supported IDEs

- Visual Studio Code version 1.46.0 or higher.
- Github Codespaces

### Supported File Types

The extension is activated for COBOL files with the following file extensions:
 - .cobol
 - .cob
 - .cbl

### Compatibility

The COBOL Control Flow extension is not compatible with other extensions that provide COBOL support except COBOL Language Support. We recommend that you disable all other COBOL-related extensions to ensure that COBOL Control Flow functions correctly.

### Integration with COBOL Language Support

We recommend that you download and install [COBOL Language Support](https://marketplace.visualstudio.com/items?itemName=broadcomMFD.COBOL-language-support) to enhance the functionality of COBOL Control Flow. Advantages of integrating COBOL Control Flow with COBOL Language Support include:

- Support for other dialects of COBOL such as IDMS and MAID
- Support for copybooks, including IDMS copybooks, stored both locally in your workspace and on mainframe data sets
- Support for EXEC CICS and EXEC SQL statements
- More precise graphs generated by the COBOL Language Support code parser

## Using COBOL Control Flow

###  Generate a COBOL Control Graph

To use the COBOL Control Flow interactive graph, generate it in the VS Code interface.
![](https://github.com/BroadcomMFD/cobol-control-flow/blob/master/CobolControlFlow_generateFlow.gif?raw=true)

**Follow these steps:**
1. Open a COBOL file.
2. Right click inside the file editor.
    - The context menu opens.
3. Select **Generate COBOL Control Flow**.
    - The COBOL Control Flow graph is generated and displayed in a new window located to the side of the COBOL file.

### Navigate Through the Code Using the COBOL Control Graph

Once the COBOL Control Flow graph is generated you can navigate through the COBOL code by clicking on the individual nodes in the graph.

![](https://github.com/BroadcomMFD/cobol-control-flow/blob/master/CobolControlFlow_highlightingCode.gif?raw=true)

You can also click anywhere in the COBOL code to navigate to the relevant node in the graph.
    
### Display Tooltips

Hover over a node in the COBOL Control Flow graph to display the first several lines of the corresponding paragraph.

![](https://github.com/BroadcomMFD/cobol-control-flow/blob/master/CobolControlFlow_tooltip.gif?raw=true)

## Copybook Support

COBOL Control Flow displays copybooks, including IDMS copybooks, on the interactive graph, as long as you have the COBOL Language Support extension installed and configured. You can configure COBOL Language Support to look for copybooks that are stored locally, or retrieve copybooks from mainframe data sets. To retrieve copybooks from mainframe data sets, the [Zowe Explorer](https://marketplace.visualstudio.com/items?itemName=Zowe.vscode-extension-for-zowe) extension is also required.

For instructions on how to set paths to your copybook folders, see the **Copybook Support** section of the **[COBOL Language Support documentation](https://github.com/eclipse/che-che4z-lsp-for-cobol#readme)**.

## Technical Assistance and Support for COBOL Control Flow

The COBOL Control Flow extension is made available to customers on the Visual Studio Code Marketplace in accordance with the terms and conditions contained in the provided End-User License Agreement (EULA).

If you are on active support for Brightside, you get technical assistance and support in accordance with the terms, guidelines, details, and parameters that are located within the Broadcom [Working with Support](https://support.broadcom.com/external/content/release-announcements/CA-Support-Policies/6933) guide.

This support generally includes:

* Telephone and online access to technical support
* Ability to submit new incidents 24x7x365
* 24x7x365 continuous support for Severity 1 incidents
* 24x7x365 access to Broadcom Support
* Interactive remote diagnostic support
* Technical support cases must be submitted to Broadcom in accordance with guidance provided in “Working with Support”.

Note: To receive technical assistance and support, you must remain compliant with “Working with Support”, be current on all applicable licensing and maintenance requirements, and maintain an environment in which all computer hardware, operating systems, and third party software associated with the affected Broadcom software are on the releases and version levels from the manufacturer that Broadcom designates as compatible with the software. Changes you elect to make to your operating environment could detrimentally affect the performance of Broadcom software and Broadcom shall not be responsible for these effects or any resulting degradation in performance of the Broadcom software. Severity 1 cases must be opened via telephone and elevations of lower severity incidents to Severity 1 status must be requested via telephone.

## Privacy Notice
The extensions for Visual Studio Code developed by Broadcom Inc., including its corporate affiliates and subsidiaries, ("Broadcom") are provided free of charge, but in order to better understand and meet its users’ needs, Broadcom may collect, use, analyze and retain anonymous users’ metadata and interaction data, (collectively, “Usage Data”) and aggregate such Usage Data with similar Usage Data of other Broadcom customers. Please find more detailed information in License and Service Terms & Repository.

This data collection uses built-in Microsoft VS Code Telemetry, which can be disabled, at your sole discretion, if you do not want to send Usage Data.

The current release of COBOL Control Flow collects anonymous data for the following events:
- Activation of this VS Code extension
- Interaction with the nodes
- Use of zoom
- Collapse and expand of graph edges
- Count of lines of analyzed COBOL file (Performance)
- Parsing time (Performance)
- Rendering time (Performance)
- Errors

Each such event is logged with the following information:
- Event time
- Operating system and version
- Country or region
- Anonymous user and session ID
- Version numbers of Microsoft VS Code and COBOL Control Flow
