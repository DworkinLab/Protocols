# Some notes I made from the in lab training on the Eppendorf Realplex.

There is a shortcut to the users manual with more detail on this the desktop.

1.	Turn on Realplex prior to the computer.
2.	Click on the Realplex icon -> open V1.5 (updates are free contact Jason or Rob)
3.	Database backend automatically loads (based on Firebird)

Users – The Eppendorf User is a generic user with admin privileges.
 For each lab create a single user that is “standard user” not admin. Please contact me to set up new lab users.
  Within each user, individual folders can be set up for each lab user.

The database currently backs up all data files once/week. However since the computer is not networked, we need to manually backup data (files are quite small, so a thumb drive will get them all).

  When a user is logged in, and you are at the main interface for the Realplex software, look in the toolbar for a “play” icon (triangle). If it is green then the computer is communicating with the realplex cycler. If it is grayed out it is not.

Note: In the lower right corner is the hint window which provides hints for each step in the process.


4.	Select dye – FAM for TAQMAN, SYBR or VIC/Yakami
5.	Open up plate layout.
6.	Select wells for part of an assay (unknown, neg. control, pos control, standard curve).
7.	 Then either click the icon in the shortcut toolbar or right click mouse to pick type (referring to unknown, controls etc..).
8.	For Units – pick (copies, conc etc…) For relative expression it will not matter.
9.	Set up plate, there are a number of functions to speed up the process. i.e. if you select 9 well, choose “standard curve” and 3 replicates then with 3 conc it should assign it on the plate. Read more in the manual on this.
10.	 You can if you want create sub-assays on the plate.
11.	Probe (pick probe – SYBR green most likely)
12.	Background – currently only calibrated for “clear” plates, if you are using white plates see manual for calibration.

Note- What is optically important is the optical “seal”. The thermal plate sealing method is preferred especially for low volume reactions (5-10 microL), optically clear caps is next (and apparently fits on the plates), followed by adhesive based seals.

Note – To Calibrate for “white” background plates, please contact Rob or Jason, to walk you through the procedure.  Use TE pH8.0  10mM.

Note – Setting up plates : Default settings you way wish to change the hot start option (default 2 minutes, possibly requires longer)and extension temperature. Indeed given that amplicons will generally be in the 80-150bp range,  the default annealing, extension and melting times may be all a bit overkill. Must be empirically set.

Note – The lighting bolt indicates when the LED array “flashes” to get an input. This is by default during the extension phase of each cycle.

13.	Right click to add melting curve. (Note if you see evidence of primer dimer, decrease the primer concentration).
14.	 Always keep the “lid temperature” option on, and set to 105.
15.	If you are going to have a low temperature hold, set this to 10 Degrees C, not 4!!!
Indeed for all thermocyclers it should be 10, and not 4. (The default is 4, but change it to 10).
16.	If you are using a low temperature hold for the final step, switch “off lid @ low temp” button.
17.	 Run as gradient if you are testing primer conditions (click button). This can be important on the “S” block since this ramps very quickly, and so requires more precise annealing temperatures to be set. If you want to use an old program as the basis for a current experiment, click the “simulate mastercycler” button to slow down the ramping speed.
        
    Note: To use the Realplex as a traditional thermocycler, do not make any plate layout, and remove the LED excitation step (lightning bolt).

     Note: “impulse feature” is essentially an overdrive step for ramp speed only for the first cycle to act as a hardware mediated hotstart to prevent non-specific amplification. Most RT mastermixes come with hotstart enzyme so this is not necessary.

18.	Set control to “simulated tube”, not block.
19.	Press start. Create New Folder if Nescessary. Name Assay. If desired set as a template.

Analysis 

Log versus linear button for choosing visualization. The Red line represents the ct value.

Baseline setting: For SYBR green it is recommended to use the automatic baseline. For TAQMAN the manual or 3-15 setting is preferred since the first cycle can sometimes have some autofluorescence.

In Picking Baseline and Threshold optimize around both efficiency and R2.
For threshold currently noiseband or R2 are recommended. The other algorithms have not yet been published so they represent a blackbox.

For a standard curve the “y –intercept” represents the highest ct value that is biologically meaningful. Any ct value below that (and above background) represents true biological signal, although not necessarly optimized (baseline and threshold for that).

Under the drop down menu “type of application” You can also access melting curve information to look for any secondary amplicons.

Data can be copy and pasted into excel or as tab delimited into notepad. Highlight the data on the left, right click and press copy all.

The export function is useful for bringing data to another computer with the software. It uses a .asy (Eppendorf) file format, although Microsoft sometimes tries to use that extension as well.

If you want to a PDF report of all data, figures etc… (for archival purposes).
File -> report -> highlight the useful columns (probably all) and save as a PDF. 


Relative Quantification

Plate set up
Choose Dye.
For the reference gene, make sure  that the “housekeeping gene” box is checked. This tells the software that this is relative quantification. Set up control and experimental conditions as normal (make sure housekeeping gene is not highlighted for the gene of interest). Once all of the genes of interest (and reference) and conditions are set,  in the shortcut toolbar click the “link” feature so that control versus treated can be linked with references. Read manual for more details.

If the delta-delta ct method is being used, make sure that the control/untreated group is labeled as “calibration”.

Analysis
In the “type of application” drop down menu choose the relative quantification option.

   

