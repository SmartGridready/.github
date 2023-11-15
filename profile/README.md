### Welcome to the SmartGridready software repository

SmartGridready is the label for standardized, secure communication between products, systems and electricity networks.
You find further information about SmartGridready on our [SmartGridready](https://smartgridready.ch/) website.

SmartGridready provides you a software stack that enables easy integration of SmartGridready compliant products/devices
into communicator and controlling applications such as energy-managers and network flexibility managers:

![SmartGridready architecture](doc/architecture.png)

*Figure 1 Basic SmartGridready architecture. Refer to the readme's of the projects 
<a href="https://github.com/SmartGridready/SGrSpecifications/">SGrSpecifications</a>,
<a href="https://github.com/SmartGridready/SGrJavaSamples">SGrJavaSamples</a> and
<a href="https://github.com/SmartGridready/SGrJavaDrivers">SGrJavaDrivers</a> for detailed description.*

#### The software projects below target different user groups:
- Developers of SmartGridready client devices, called in **communicator** in SmartgridReady terminology. They are users of the SmarGridready **commhandler** library.
- Developers of SmartGridready core library components, called **commhandler** in SmartgridReady terminology. They are contributors to the SmartGridready opensource software stack. 
- Developers of device drivers who want to integrate their own device driver (e.g. modbus driver) into the SmartgridReady software stack. They may contribute their own driver to the SmartGridready opensource software stack.

### Project descriptions
<table>
    <tr><th>Project</th><th>Target User Group</th><th>Description</th></tr>
    <tr>
        <td><a href="https://github.com/SmartGridready/SGrSpecifications/">SGrSpecifications</a></td>
        <td>All developers</td>
        <td>SGrSpecifications defines the XML-schemas for the SmartGridready functional-profiles and the XML-schemas for 
        device descriptions in XML, called EI-xml (external interface XML). 
        It also contains the EI-xml for SmartGridready certified devices.</td>
    </tr>
    <tr>
        <td><a href="https://github.com/SmartGridready/SGrJavaSamples">SGrJavaSamples</a></td>
        <td>Communicator Developers</td>
        <td>SGrJavaSamples provides starter projects for communicator developers. The projects provides
        samples on how to use the SmartgridReady API. The samples describe how load a device description EI-xml, 
        read/write device data-points, handle specific datatypes such as arrays, enums and bitmaps. Furthermore
        ther are samples on how you can use the commhandler library using asynchronous programming. 
        </td>
    </tr>
    <tr>
        <td><a href="https://github.com/SmartGridready/SGrJava">SGrJava</a></td>
        <td>SmartGridready core developers</td>
        <td>SGrJava provides the commhandler core library code. The commhandler core provides the
        conversion of the generic SmartGridready API to the specific device API based on the EI-xml
        device description files.</td>
    </tr>
    <tr>
        <td><a href="https://github.com/SmartGridready/SGrJavaDrivers">SGrJavaDrivers</a></td>
        <td>SmartGridReady core developers, 3rd party device driver developers</td>
        <td>Within the SGrJavaDrivers project you find the device driver adapter interface specification
        (Java interface) and a concrete Implementation of a modbus interface driver called 'EasyModbus'.
        </td>
    </tr>
    <tr>
        <td><a href="https://github.com/SmartGridready/SGrPython">SGrPython</a></td>
        <td>All developers that use Python as programming language</td>
        <td>SGrPython provides a commhandler library written in Python. It also contains an example folder
        with code samples on how to use the commhandler library API within communicator applications.</td>
    </tr>
</table>
