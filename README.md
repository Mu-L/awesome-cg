Contents
-----------
* Books
  * [GPU Details](#gpudetail)
* Physically-based Rendering
  * [Getting Starting](#gettingstarted)
  * [BRDF/BSDF/BSSRDF](#brdf)
  * [Importance Sampling](#importancesampling)
  * [Low-discrepancy sequences](#low-discrepancysequences)
  * [Path Tracing](#pathtracing)
  * [Denoise](#denoise)
* Real Time Rendering
  * [Learn OpenGL](#learnopengl)
  * [Lighting](#lighting)
  * [Global Illumination](#globalillumination)
  * [Volumetric Lighting](#volumetriclighting)
  * [Shadow](#shadow)
  * [Terrain](#terrain)
  * [Texture/Normal/Parrlax/Filter](#texture)
  * [Atmospheric Scattering](#atmosphericscattering)
  * Post Process
    * [Screen Space Reflections](#screenspacereflections)
    * [Depth Of Filed](#depthoffiled)
    * [HDR/Bloom](#bloom)
    * [Tone Mapping](#tonemapping)
    * [Color Grading & Correction](#colorgradingcorrection)
    * [Anti-aliasing](#anti-aliasing)
* [Color Encoding](#colorencoding)
* [Performance profile](#performanceprofile)

### Getting&nbsp;Started
----------
* [如何看懂这些"该死的"图形学公式](https://zhuanlan.zhihu.com/p/21489591)
* [The Rendering Equation](http://www.dca.fee.unicamp.br/~leopini/DISCIPLINAS/IA725/ia725-12010/kajiya-SIG86-p143.pdf)

### BRDF
--------
* [Cook-Torrance - A Reflectance Model for Computer Graphics](http://inst.eecs.berkeley.edu/~cs283/sp13/lectures/cookpaper.pdf)
* [Cook-Torrance 模型公式推导](https://www.cnblogs.com/herenzhiming/articles/5789043.html)
* [Blinn-phong - ](https://design.osu.edu/carlson/history/PDFs/blinn-light.pdf)
* [GGX - Microfacet Models for Refraction through Rough Surfaces](http://www.cs.cornell.edu/~srm/publications/EGSR07-btdf.pdf)
* [An Illumination Model for a Skin Layer Bounded by Rough Surfaces](http://www.dgp.toronto.edu/people/stam/reality/Research/pdf/skin.pdf)

### Importance&nbsp;Sampling
----------
* [GPU-Based Importance Sampling](https://developer.nvidia.com/gpugems/GPUGems3/gpugems3_ch20.html) GPU Gems 3 - Chapter 20.
* [Importance Sampling for Production Rendering](http://www.igorsklyar.com/system/documents/papers/4/fiscourse.comp.pdf)
* [Monte Carlo Techniques for Direct Lighting Calculations](http://www.cs.utah.edu/~shirley/papers/tog94.pdf)

### Low-discrepancy&nbsp;sequences
----------
* [低差异序列（一）- 常见序列的定义及性质](https://zhuanlan.zhihu.com/p/20197323)
* [低差异序列（二）- 高效实现以及应用](https://zhuanlan.zhihu.com/p/20374706)
* [Quasi-Monte Carlo Image Synthesis
in a Nutshell](http://web.maths.unsw.edu.au/~josefdick/MCQMC_Proceedings/MCQMC_Proceedings_2012_Preprints/100_Keller_tutorial.pdf)
* [Enumerating Quasi-Monte Carlo Point
Sequences in Elementary Intervals](http://gruenschloss.org/sample-enum/sample-enum.pdf)
* [Efficient Multidimensional Sampling](https://www.uni-kl.de/AG-Heinrich/EMS.pdf)
* [Blog - Leonhard](http://gruenschloss.org/)

### Path&nbsp;Tracing
----------
* [Simple PathTracing by Inigo Quilez](http://www.iquilezles.org/www/articles/simplepathtracing/simplepathtracing.htm)
* [Efficient Monte Carlo Rendering with Realistic Lenses](https://cg.ivd.kit.edu/publications/pubhanika/2014_lenssim.pdf)

### Denoise
----------
* [A Machine Learning Approach for Filtering Monte Carlo Noise](http://cvc.ucsb.edu/graphics/Papers/SIGGRAPH2015_LBF/)

### LearnOpenGL
---------
* [Learn Opengl](https://learnopengl.com/)
* [Learn Opengl - Zh-cn](https://learnopengl-cn.github.io/)

### Lighting
----------
* Approximation of the IBL’s DFG term for a cloth BRDF \[[Github](https://gist.github.com/romainguy/52d0e7f070d9ed7b44a0327d735fe33e)\]
* [Pre-Integrated Skin Shading](http://simonstechblog.blogspot.com/2015/02/pre-integrated-skin-shading.html)
* [Real-Time Polygonal-Light Shading with Linearly Transformed Cosines](https://eheitzresearch.wordpress.com/415-2/) \[[Source Code](https://github.com/selfshadow/ltc_code)]
* [Special-Case Materials Wetness ](http://advances.realtimerendering.com/other/2016/naughty_dog/NaughtyDog_TechArt_Final.pdf)
* [Matcap - Creating a Spherical Reflection/Environment Mapping shader ](https://www.clicktorelease.com/blog/creating-spherical-environment-mapping-shader/)

### Shadow
----------
* [Shadow Map Antialiasing (PCF)](https://developer.nvidia.com/gpugems/GPUGems/gpugems_ch11.html) GPU Gems 1 - Chapter 11.
* [Summed-Area Variance Shadow Maps (VSM)](https://developer.nvidia.com/gpugems/GPUGems3/gpugems3_ch08.html) GPU Gems 3 - Chapter 08.
* [Parallel-Split Shadow Maps on Programmable GPUs (PSSM)](https://developer.nvidia.com/gpugems/GPUGems3/gpugems3_ch10.html) GPU Gems 3 - Chapter 10.
* [Percentage-Closer Soft Shadows (PCSS)](http://developer.download.nvidia.com/shaderlibrary/docs/shadow_PCSS.pdf) Randima Fernando NVIDIA Corporation

### Volumetric&nbsp;Lighting
* [游戏开发相关实时渲染技术之体积光](https://zhuanlan.zhihu.com/p/21425792)
* [Volumetric Light Scattering as a Post-Process](https://developer.nvidia.com/gpugems/GPUGems3/gpugems3_ch13.html) GPU Gems 3 - Chapter 13.

### Global&nbsp;Illumination
-----------
* [Point Based Global Illumination](http://www.aduprat.com/portfolio/?page=articles/PBGI)] \[[Github](https://github.com/XT95/PBGI)]
* [Light-Propagation-Volumes](http://www.crytek.com/download/Light_Propagation_Volumes.pdf) \[[Github](https://github.com/Global-Illuminati/Light-Propagation-Volumes)]
* [Webgl-deferred-irradiance-volume](http://codeflow.org/entries/2012/aug/25/webgl-deferred-irradiance-volumes/) \[[Github](https://github.com/pyalot/webgl-deferred-irradiance-volumes)]
* [Real-Time Global Illumination using Precomputed Light Field Probes](http://research.nvidia.com/sites/default/files/pubs/2017-02_Real-Time-Global-Illumination/light-field-probes-final.pdf) \[[Github](https://github.com/Global-Illuminati/Precomputed-Light-Field-Probes)\]
* [Real-time Global Illumination by Precomputed Local Reconstruction from Sparse Radiance Probes](https://users.aalto.fi/~silvena4/Projects/RTGI/index.html) \[[Github](https://github.com/Global-Illuminati/Precomputed-Local-Reconstuction-from-Sparse-Radience-Probes)\]
 
### Terrain
----------
* [Fast Terrain Rendering Using Geometrical MipMapping](https://www.flipcode.com/archives/article_geomipmaps.pdf)
* [Real-time optimally adapting mesh (ROAM)](https://www.hindawi.com/journals/ijcgt/2008/753584/) \[[Source Code](http://www.cognigraph.com/ROAM_homepage/ROAM2/)]
* [Chunked LOD](http://tulrich.com/textweb.pl?path=geekstuff/chunklod.txt)
* [Terrain Rendering Using GPU-Based Geometry Clipmaps](https://developer.nvidia.com/gpugems/GPUGems2/gpugems2_chapter02.html) GPU Gems 2 - Chapter 02.
* [Procedural Modeling and Rendering of Cities](http://pcity.sourceforge.net/)

### Texture
----------
* [Parallax Occlusion Map](http://sunandblackcat.com/tipFullView.php?topicid=28)
* [Normal Blending in Detail](http://blog.selfshadow.com/publications/blending-in-detail/)
* [Bump map to Normal](https://docs.unrealengine.com/latest/attachments/Engine/Rendering/LightingAndShadows/BumpMappingWithoutTangentSpace/mm_sfgrad_bump.pdf)
* [Fast Filter-Width Estimates with Texture Maps](https://developer.nvidia.com/gpugems/GPUGems/gpugems_ch25.html) GPU Gems 1 - Chapter 25.

### Atmospheric&nbsp;Scattering
----------
* [Accurate Atmospheric Scattering](https://developer.nvidia.com/gpugems/GPUGems2/gpugems2_chapter16.html) GPU Gems 2 - Chapter 16.
* [An Approximation to the Chapman Grazing-Incidence Function for Atmospheric Scattering](http://www.gameenginegems.net/gemsdb/article.php?id=1133) \[[Source Code](https://www.shadertoy.com/view/XlBfRD)] GPU Pro 3
* [Precomputed Atmospheric Scattering](https://ebruneton.github.io/precomputed_atmospheric_scattering/) \[[Source Code](https://github.com/ebruneton/precomputed_atmospheric_scattering)]
* [Wavelength dependency of the Solar limb darkening](http://www.physics.hmc.edu/faculty/esin/a101/limbdarkening.pdf)
* [Volumetric Atmospheric Scattering](https://www.alanzucconi.com/2017/10/10/atmospheric-scattering-1/) Alan Zucconi

### Screen&nbsp;Space&nbsp;Reflections
----------
* [Screen Space Glossy Reflections](http://roar11.com/2015/07/screen-space-glossy-reflections/)

### Depth&nbsp;of&nbsp;Filed
----------
* [Depth of Field: A Survey of Techniques](https://developer.nvidia.com/gpugems/GPUGems/gpugems_ch23.html)
* [Practical Post-Process Depth of Field](https://developer.nvidia.com/gpugems/GPUGems3/gpugems3_ch28.html)
* [Hexagonal Bokeh Blur Revisited](https://colinbarrebrisebois.com/2017/04/18/hexagonal-bokeh-blur-revisited/) \[[Source Code](https://github.com/zigguratvertigo/HexBokehBlur)]

### Bloom
----------
* [Real-Time Glow](https://developer.nvidia.com/gpugems/GPUGems/gpugems_ch21.html) GPU Gems 1 - Chapter 21.
* [How to do good bloom for hdr rendering](http://kalogirou.net/2006/05/20/how-to-do-good-bloom-for-hdr-rendering/)
* [Dirt Mask Image Best Practices](https://docs.unrealengine.com/en-us/Engine/Rendering/PostProcessEffects/Bloom) Unreal 4

### Tonemapping
----------
* [ACES Filmic Tone Mapping Curve](https://knarkowicz.wordpress.com/2016/08/31/hdr-display-first-steps/)

### Color&nbsp;Grading&nbsp;&&nbsp;Correction
----------
* [The Importance of Being Linear](https://developer.nvidia.com/gpugems/GPUGems3/gpugems3_ch24.html) GPU Gems 3 - Chapter 24.
* [Using Lookup Tables to Accelerate Color Transformations](https://developer.nvidia.com/gpugems/GPUGems2/gpugems2_chapter24.html) GPU Gems 2 - Chapter 24.

### Color&nbsp;Encoding
----------
* [RGBM color encoding](http://graphicrants.blogspot.com/2009/04/rgbm-color-encoding.html)
* [Compact YCoCg Frame Buffer for small IBL-Buffer](http://jcgt.org/published/0001/01/02/)
* [Compact Normal Storage for small G-Buffers](http://aras-p.info/texts/CompactNormalStorage.html)
* [Convert Temperature to RGB](https://github.com/davidf2281/ColorTempToRGB)

### Anti-aliasing
-------
* [Geometric Specular Aliasing](http://media.steampowered.com/apps/valve/2015/Alex_Vlachos_Advanced_VR_Rendering_GDC2015.pdf)

### Performance&nbsp;Profile
-------
* [Screen-filling Rasterization using Screen-aligned Quads and Triangles](https://cginternals.com/en/blog/2018-01-10-screen-aligned-quads-and-triangles.html)

### GPU&nbsp;Detail
----
* [A-trip-through-the-graphics-pipeline](https://github.com/alaingalvan/a-trip-through-the-graphics-pipeline-book)

### Paper
----
* [原神](https://zhuanlan.zhihu.com/p/316138540)
