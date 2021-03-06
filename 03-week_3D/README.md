## Today
- review homework
- Rhino Q & A tutorials
- sketches (upload to class share folder)
- 3D printing demo
- work time
    - modeling
    - printing


# 3D printing
Customization is a product of 3D printing technologies. The idea that parts can be made special with a few parameters changed, interchangable parts leads to endless possibilities

![Danit Peleg](https://danitpeleg.com/wp-content/uploads/2017/07/danit-peleg-venus-3.jpg)

[Danit Peleg](https://danitpeleg.com/) Designs 3D printable, wearable fashion. Now available, a customizable 3d printed jacket.

Enabling customizable prosthetics to be accessible and affordable
[Here is a link](http://www.danaeprosthetics.com/) to the website of some MICA alumns who received an up-start grant for their prosthetics design software.

![prosthetics](https://img.newatlas.com/exo-prosthetic-leg-low-cost-beautiful-22.JPG?auto=format%2Ccompress&ch=Width%2CDPR&crop=entropy&dpr=2&fit=crop&h=347&q=40&w=616&s=65ff5819e318d9d82fe99f3d2d645a33)

[Article here](http://newatlas.com/exo-prosthetic-leg-3d-printing/35297/)

And 3d printed Organs!
Organs that have been successfully printed and implemented in a clinical setting are either flat, such as skin, vascular, such as blood vessels, or hollow, such as the bladder. When artificial organs are prepared for transplantation, they are often produced with the recipient's own cells.

![Ear](https://3dprint.com/wp-content/uploads/2016/02/ears.png)

## FDM
Fused deposition modeling (FDM) is an additive manufacturing (AM) technology commonly used for modeling, prototyping, and production applications. The exactly equivalent term, fused filament fabrication (FFF), was coined by the members of the RepRap project. It is also sometimes called Plastic Jet Printing (PJP).

## Design for 3D Printing
### Overhangs

An overhang is where the printed layer of material is only partially supported by the layer below or not supported at all. All printer technologies are based on an additive process, with the layer about to be printed requiring a layer below it to adhere to (with the exceptions of SLS and Binder Jetting). There are limits that printers can print up to, 45 degrees for FDM, beyond which support material is needed to support overhangs and allow them to be printed accurately.

![overhangs](https://s3-eu-west-1.amazonaws.com/3dhubs-knowledgebase/key-design-considerations-for-3d-printing/photo5.jpg)

### Wall thickness

In order to print layer upon layer, it’s necessary to have a minimum wall thickness, depending on the 3D printing technique that you use.

### Warping

3D printing techniques rely on heating up the material to over 200 ℃ to either melt or sinter material. The heating up and cooling down of material can cause some warping of the 3D print. Long, flat surfaces can be especially prone to warping. Warping can typically be avoided by using correct machine calibration and having adequate surface adhesion between your part and the print bed. A few ways to avoid warping are to design something that is open on the print surface or to break it into parts if it is big and flat on the bottom.

## Water Tight

Any models that are intended to be used for 3D printing should be completely manifold (watertight). Every edge on your model should have exactly 2 polygons attached to it and include no holes. Models that are not manifold (watertight) might get misinterpreted by the software that generates the instructions for the 3D printer (slicer software). This might results in the object having inconsistent layers, holes or cause the model to be unprintable.

Non-manifold issues are often not visible to the at the modeling stage. Use SelOpenPolysurf to find any open surfaces when you are modeling in Rhino.

## Orientation

Often a lot of time is spent determining the optimal part orientation to reduce the likelihood of print failure and the amount of support material that is being used.
In general the top or upward facing surface of a 3D print will have the best surface finish.
The bottom where it meets the bed surface will be the smoothest.

## Prusa i3 MK2

After building a design in Rhino, you will export your file as an .STL (stereolithography) file. STL uses triangles (polygons) to describe the surfaces of an object. A box will pop up after you export asking you to set your tolerance. A mesh tolerance that is less complicated (0.1) is easier to process, but you will see the triangles of the mesh more; the smaller the tolerance (.001) is more complicated but higher resolution.  Exporting with a tolerance smaller than 0.001 mm won’t increase the quality of your print because printers are not able to print in that detail.

Create GCode:

G-code is a numerical control (NC) programming language. It is used in computer-aided manufacturing (CAM) to control automated machine tools (including CNC machines and 3D printers). The slicer program also allows the designer to customize the build parameters including support, layer height, and part orientation.

- Open Slicer
- Check which printer you are on and select that printer (mk2 or mk3)
- Set the settings to "fast"
- You may want to alter print settings:
  - You can lower your infill density to 10% or so. This will help your print go faster. If you want a heavier print that is denser, you will want to increase the percentage, but remember that it will increase your print time and use more material.
  - A skirt can be used to help limit warping.
- Always check with your manufacturer about filament settings, but if you are using inland PLA it will be the standard settings
- Plater: Add your STL file
- Slice Now
- You can preview your file layer by layer to check for any issues
- Insert the SD card and Export GCode to the card
- LET A TECH TO HELP REMOVE YOUR PRINT from the orange Prusas... The membrane of the heated beds are easy to damage

## Resources

[3D Hubs](https://www.3dhubs.com/knowledge-base/how-design-snap-fit-joints-3d-printing) is a great source for more information about 3d printing, and this link will take you to some snap-fit joint and living hinge exercises


## Homework

- complete object copy and 3D print
  - take a quality photo of your completed piece next to the original object; upload the image(s) and your Rhino file to the class Homework Drive
- read Sean Ragan’s two articles on CNC joinery in Make Magazine
[CNC Panel Joinery Notebook](https://makezine.com/2012/04/13/cnc-panel-joinery-notebook/)
[CNC Joinery Notebook: Update 1](https://makezine.com/2013/01/25/cnc-joinery-notebook-update-1/)
- read pgs 1-22 of the [RhinoCAM 2015 Mill Reference](https://mecsoft.com/wp-content/uploads/2015/09/RhinoCAM_2015_MILL-Reference_Sample.pdf)
