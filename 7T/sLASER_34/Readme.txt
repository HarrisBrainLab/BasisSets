These basis sets contains the following components:

Alanine, Aspartate, Choline (Cho), Glycerophosphochoine (GPC), Phosphocholine (PC), Creatine (Cr), Phosphocreatine (PCr), GABA, Glutamate (Glu), Glutamine (Gln), Lactate, Myo-Inisitol, N-acetylaspartate (NAA), n-acetylaspartylglutamate (NAAG), Scyllo-Inositol, Glutathione (GSH), Glucose, Taurine, beta-hydroxybutyrate, Cit, Eth, Glycine, PE. 

The basis set Siemens_7T_slaser_34_MM also includes nine macromolecules (M0.95, M1.24, M1.43, M1.71, M2.07, M2.30, M3.03, M3.24, M3.98) simulated as detailed in Bell et al. (2024) under review (details and spin systems can be found in https://github.com/HarrisBrainLab/MMSim).

The components of this basis set were simulated using the FID-A script run_simSteamShaped_fast with the parameters detailed below. 

% ************INPUT PARAMETERS**********************************
n=8224; %= number of points in fid/spectrum
sw=10000; %= desired spectral width in [Hz]
Bfield=6.98; %= main magnetic field strength in [T]
%lw=2; %= linewidth in [Hz]
rfPulse=io_loadRFwaveform_09197('sampleAFPpulse_HS2_R15.RF','inv'); % adiabatic RF pulse shaped waveform % TB hardcode w1max to 0.9197
refTp=3.5; %= RF pulse duration in [ms]
flipAngle=180; %= flip angle of refocusing pulses [degrees] (Optional.  Default = 180 deg)
centreFreq=2.3; %= centre frequency of the spectrum in [ppm] (Optional.  Default = 2.3)
thkX=2.5; %slice thickness of x refocusing pulse [cm]
thkY=2.5; %slice thickness of y refocusing pulse [cm]
fovX=3; %size of the full simulation Field of View in the x-direction [cm]
fovY=3; %size of the full simulation Field of View in the y-direction [cm]
nX=32; %Number of grid points to simulate in the x-direction
nY=32; %Number of grid points to simulate in the y-direction
te=34;         %semiLASER total echo time [ms]
% ************END OF INPUT PARAMETERS**********************************

 
