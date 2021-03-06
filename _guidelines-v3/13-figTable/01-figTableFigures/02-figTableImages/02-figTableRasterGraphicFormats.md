---
sectionid: figTableRasterGraphicFormats
title: "Raster Graphic Formats"
version: "v3"
---



<table class="table table-striped">
   <thead>
      <tr>
         <th>Value</th>
         <th>Description</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>PNG: Portable Network Graphics format</td>
         <td> - PNG is a non-proprietary raster format currently widely available. It provides
            an
            extensible file format for the losslessly compressed storage of raster images.
            Indexed-color, grayscale, and true-color images are supported, plus an optional alpha
            channel. Sample depths range from 1 to 16 bits. It is defined by IETF RFC 2083, March
            1997.
         </td>
      </tr>
      <tr>
         <td>TIFF: Tagged Image File Format</td>
         <td> - Currently the most widely supported raster image format, especially for black and
            white images, TIFF is also one of the few formats commonly supported on more than
            one
            operating system. The drawback to TIFF is that it actually is a wrapper for several
            formats, and some TIFF-supporting software does not support all variants. TIFF files
            may
            use LZW, CCITT Group 4, or PackBits compression methods, or may use no compression
            at
            all. Also, TIFF files may be monochrome, greyscale, or polychromatic. All such options
            should be specified in prose at the end of the <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/encodingDesc.html">encodingDesc</a>
            section of the MEI header for any document including TIFF images. TIFF is owned by
            Aldus
            Corporation. Documentation on TIFF is available from the owner at Craigcook Castle,
            Craigcook Road, Edinburgh EH4 3UH, Scotland, or 411 First Avenue South, Seattle,
            Washington 98104 USA.
         </td>
      </tr>
      <tr>
         <td>GIF: Graphics Interchange Format</td>
         <td> - Raster images are widely available in this form, which was created by CompuServe
            Information Services, but has by now been implemented for many other systems as well.
            Documentation is copyright by, and is available from, CompuServe Incorporated, Graphics
            Technology Department, 5000 Arlington Center Boulevard, Columbus, Ohio 43220 USA.
            
         </td>
      </tr>
      <tr>
         <td>PBM: Portable Bit Map</td>
         <td> - PBM files are easy to process, eschewing all compression in favor of transparency
            of file format. PBM files can, of course, be compressed by generic file-compression
            tools for storage and transfer. Public domain software exists which will convert many
            other formats to and from PBM. Documentation of PBM is copyright by Jeff Poskanzer,
            and
            is available widely on the Internet.
         </td>
      </tr>
      <tr>
         <td>PCX: IBM PC raster format</td>
         <td> - This format is used by most IBM PC paint programs, and supports both monochrome
            and polychromatic images. Documentation is available from ZSoft Corporation, Technical
            Support Department, ATTN: Technical Reference Manual, 450 Franklin Rd. Suite 100,
            Marietta, GA 30067 USA.
         </td>
      </tr>
      <tr>
         <td>BMP: Microsoft bitmap format</td>
         <td> - This format is the standard raster format for computer using Microsoft Windows
            (tm) or Presentation Manager (tm). Documentation is available from Microsoft
            Corporation. 
         </td>
      </tr>
   </tbody>
</table>
