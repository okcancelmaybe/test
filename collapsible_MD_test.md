# .NET API for 3D File Formats

[![Nuget](https://img.shields.io/nuget/v/Aspose.3D)](https://www.nuget.org/packages/Aspose.3D/) ![Nuget](https://img.shields.io/nuget/dt/Aspose.3D)

[![Banner](https://www.dropbox.com/s/gsymp1t927ebjaw/aspose_3d-for-net-banner-e-5.png?raw=1)](https://downloads.aspose.com/3d/net)

[Product Page](https://products.aspose.com/3d/net/) | [Docs](https://docs.aspose.com/3d/net/) | [Demos](https://products.aspose.app/3d/family) | [API Reference](https://apireference.aspose.com/3d/net) | [Examples](https://github.com/aspose-3d/Aspose.3D-for-.NET/tree/master/Examples) | [Blog](https://blog.aspose.com/category/3d/) | [Search](https://search.aspose.com/) | [Free Support](https://forum.aspose.com/c/3d) | [Temporary License](https://purchase.aspose.com/temporary-license)


<details>
<summary><b>What is Aspose.3D for .NET?</b></summary>
  
[Aspose.3D for .NET](https://products.aspose.com/3d/net/) empowers .NET applications to connect with 3D document formats. 3D .NET API lets engineers read, convert, build, alter, and control the substance of the [3D document formats](https://docs.aspose.com/3d/net/supported-file-formats/) without any 3D modeling and rendering software installed on the machine.

This on premise class library enables your .NET applications to create, read, manipulate, convert and save various formats of 3D files (e.g. 3DS, 3MF, DAE, DFX, gITF, U3D, etc.), without installing any 3rd party 3D modeling or rendering software.

It enhances your .NET apps to open files of 3D formats and work with the elements within the 3D scenes; such as; line, mesh, nurbs, curves to more complex elements like animation. You can also work with textures, parametrized geometries, scene graphs, custom properties, skeletons, morph deformers and much more.

Aspose.3D for .NET can be used on any operating system (Windows, MacOS, Linux) that can install Mono (.NET 4.0 Framework support) or use .NET Core. It is a single .NET library that you can deploy with any .NET application by simply copying it. You do not have to worry about other services or modules. Aspose.3D for .NET is designed to perform equally well on the server as well as the client-side.

</details>

<details open>
<summary><b>3D File Processing Features</b></summary>

- [Import 3D scenes from PDF](https://docs.aspose.com/3d/net/import-3d-scenes-and-contents-from-a-pdf/).
- Import, create, customize, & save 3D scenes.
- [Create 3D mesh](https://docs.aspose.com/3d/net/create-3d-mesh-and-scene/) & [scale geometries of a 3D scene](https://docs.aspose.com/3d/net/scale-geometries-of-a-3d-scene/).
- Configure cube by setting up normals or UV.
- Perform element formatting using 3D transformations.
- Share geometry data among multiple nodes of a mesh.
- [Add 3D scene animation](https://docs.aspose.com/3d/net/add-animation-property-and-setup-target-camera-in-3d-document/).
- Work with 3D objects & models.

</details>

<details open>
<summary><b>Supported File Formats</b></summary>
  
<details>
<summary>Read & Write 3D Formats</summary>

* **Autodesk** FBX 7.2 to 7.5 (ASCII/Binary)
* **3D Systems CAD:** STL (ASCII/Binary)
* **Wavefront:** OBJ
* **Discreet 3D Studio:** 3DS
* **Universal3D:** U3D
* **Collada:** DAE
* **GL Transmission:** glTF (ASCII/Binary)
* **Google Draco:** DRC
* **RVM:** (Text/Binary)
* **Portable Document Format:** PDF
* **Other:** AMF, PLY (ASCII/Binary)

</details>
  
  
  <details>
    <summary>Save 3D Files As</summary>
  
* **WEB:** HTML

</details>
  
  <details>
    <summary>Read 3D Formats</summary>
  
* **DirectX:** X (ASCII/Binary)
* **Siemens:** JT
* **Other:** DXF, ASF, VRML, 3MF

  </details>
  
</details>


<details>
<summary><b>Platform Independence</b></summary>

Aspose.3D for .NET is written in C# and supports Windows Forms as well as ASP.NET apps. Development can be performed on any platform that has a .NET environment for both 32-bit and 64-bit applications. It supports .NET Frameworks 2.0 till 4.7.2 as well as the Client Profile version for .NET Framework 4.0.
  
</details>

<details>
<summary><b>Get Started</b></summary>

Are you ready to give Aspose.3D for .NET a try? Simply execute `Install-Package Aspose.3D` from the Package Manager Console in Visual Studio to fetch the NuGet package. If you already have Aspose.3D for .NET and want to upgrade the version, please execute `Update-Package Aspose.3D` to get the latest version.

</details>

<details open>
<summary><b>Code Samples</b></summary>

<details open>
<summary>Build a Scene with Primitive 3D Models using C# Code</summary>
<p>

```csharp
// initialize a Scene object
Scene scene = new Scene();
// create a Box model
scene.RootNode.CreateChildNode("box", new Box());
// create a Cylinder model
scene.RootNode.CreateChildNode("cylinder", new Cylinder());
// save drawing in FBX format
scene.Save(dir + "output.fbx", FileFormat.FBX7500ASCII);
```
</p>
</details>

<details open>
<summary>Export 3D Scene to Compressed AMF via C# Code</summary>
<p>

```csharp
// load a scene
Scene scene = new Scene();
var box = new Box();
var tr = scene.RootNode.CreateChildNode(box).Transform;
tr.Scale = new Vector3(12, 12, 12);
tr.Translation = new Vector3(10, 0, 0);
tr = scene.RootNode.CreateChildNode(box).Transform;
// scale transform
tr.Scale = new Vector3(5, 5, 5);
// set Euler angles
tr.EulerAngles = new Vector3(50, 10, 0);
scene.RootNode.CreateChildNode();
scene.RootNode.CreateChildNode().CreateChildNode(box);
scene.RootNode.CreateChildNode().CreateChildNode(box);
// save compressed AMF file
scene.Save(dir + "output.amf", new AMFSaveOptions() {
EnableCompression = true
});
```

  </p>
</details>
  
</details>

[Product Page](https://products.aspose.com/3d/net/) | [Docs](https://docs.aspose.com/3d/net/) | [Demos](https://products.aspose.app/3d/family) | [API Reference](https://apireference.aspose.com/3d/net) | [Examples](https://github.com/aspose-3d/Aspose.3D-for-.NET/tree/master/Examples) | [Blog](https://blog.aspose.com/category/3d/) | [Search](https://search.aspose.com/) | [Free Support](https://forum.aspose.com/c/3d) | [Temporary License](https://purchase.aspose.com/temporary-license)

