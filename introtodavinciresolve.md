## MMU BA Hons FILMMAKING | INTRO TO DAVINCI RESOLVE & FCPX IMPORT/EXPORT

---

### WORKFLOW

![inline](https://dl.dropboxusercontent.com/s/ta3d9z5li2wgbap/Screenshot%202018-01-18%2008.21.21.png?dl=0)

---

### IMPORT/EXPORT PROCESS | FINAL CUT PRO

- Select project either in browser or timeline (ensure you don’t have a single clip or different project selected).
- Goto File > Export XML
- In the Metadata View dropdown menu, leave as *General*
- In the Version number, this depends on your versions of both FCPX and DaVinci Resolve. A rough pairing is as follows:

FCPX 10.4.6 | XML version 1.8 | Davinci Resolve 15
FCPX 10.4 | XML version 1.7 | DaVinci Resolve 14
FCPX 10.3 | XML version 1.6 | DaVinci Resolve 12.5
FCPX 10.2 | XML version 1.5 | DaVinci Resolve 11

If import fails, ensure you try alternate version numbers of the XML - this often solves things!

---

### IMPORT/EXPORT PROCESS | DAVINCI RESOLVE

- Goto: File > Import AAF, EDL, XML
- Navigate to your XML file from FCPX
- Leave all settings as they are (it tends to know best).
- Click OK

---

### LOG / COLOUR PROFILES

> REC709 is a monitoring standard for a final image; it is the contrast and color that generally replicates what you see to eye. But, it doesn't necessarily show everything the camera's sensor is capable of capturing. With the latest wave of Digital Cinema cameras, such as the ARRI ALEXA, the Dynamic Range detectable by our shooting devices has expanded dramatically, approaching that of film and pushing past what REC709 is capable of showing. To capture the imaging capabilities of these latest generation sensors, a LOG gamma can be used.


> There are many situations where you do not have full control over lighting conditions, such as a bright window in the background or a city street at night. Even with full control, it is still common to color correct a project once it is edited together. If the image is captured in REC709, the ability to adjust the final image is limited by the contrast range already imposed on the image. LOG is a flatter contrast, allowing far greater image manipulation. Take a look at the video to get a sense of the difference.

---

### LUTS

First of all what is a LUT and what are its typical uses?
LUT means “Look Up Table.” It’s helpful to think of it like a math problem: R= S+L
“R” being your result or what you want to attain.
“S” being your source or what you start with.
“L” being your LUT or the difference needed to make up between your source and your desired outcome.

In all cases of LUT use, the LUT is the means to make up the difference between source and result.((All cases assume the colorist (or you) is grading through a correctly calibrated monitor for evaluation and finishing. LUTs in no way replace proper calibration or color correction. They only assist in the process.)) It’s never the result by itself. How does this play out? I’ll layout a couple probably over-simplified examples:

Color Correction
A very common example is printing your final film to…real, actual film. Print film came in a variety of flavors and styles. Each style had different nuances in color. The film lab would have all that nuance information or be able to send you a print test to work with. That would be your final result. The colorist grades a picture on his calibrated monitor but if he were to send that to print, it could come out looking far different due to the nuances of the physical film.

So in our math analogy, his graded film is “S” and his film print is “R.” He then uses the information from the film lab or on his own, creates and applies the LUT or the “L” to get him from his graded film to the print and to have it look as intended after it’s on the physical film. After applying the LUT, his graded film may look awful on his monitor, but will come out correct on the film print.

---

NODE-BASED WORK FLOW



> The serial node is the most common and basic node. It is the basic building block on which most functions and operations are assigned.



![inline](https://dl.dropboxusercontent.com/s/psdimxuk0keapem/Screenshot%202018-01-24%2016.22.41.png?dl=0)

---

### LIFT GAMMA GAIN

>  Lift affects the darkest parts of your image the most, Gain affects the brightest area the most, and gamma affects the middle tones the most.


![inline](https://dl.dropboxusercontent.com/s/jtqp94lkivb0ud4/Screenshot%202018-01-24%2016.35.28.png?dl=0)

---

### SCOPES

- Waveform Monitor, and its cousin the RGB Parade
- Vectorscope
- Histogram

![inline](https://dl.dropboxusercontent.com/s/pvldrfo8tn1xs6p/Screenshot%202018-01-24%2016.14.33.png?dl=0)

---

### RESOURCES

Blackmagic DaVinci Resolve 15 | User Manual
[https://documents.blackmagicdesign.com/UserManuals/DaVinci_Resolve_15_Reference_Manual.pdf?_v=1554708500000](https://documents.blackmagicdesign.com/UserManuals/DaVinci_Resolve_15_Reference_Manual.pdf?_v=1554708500000)

Lynda.com DaVinci Tuts
[https://www.lynda.com/DaVinci-Resolve-training-tutorials/1966-0.html](https://www.lynda.com/DaVinci-Resolve-training-tutorials/1966-0.html)

---

### PRACTICAL

FULL ROUND TRIP

Using the information we've been through I would like you to:

- Import the provided XML sequence
- Grade the sequence
- Export the graded sequence as individual clips
- Re-import to FCPX
- Check timeline for any errors/issues
- Render out final Quicktime