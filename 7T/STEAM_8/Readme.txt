These basis set contains the following components:

Alanine, Aspartate, Choline (Cho), Glycerophosphochoine (GPC), Phosphocholine (PC), Creatine (Cr), Phosphocreatine (PCr), GABA, Glutamate (Glu), Glutamine (Gln), Lactate, Myo-Inisitol, N-acetylaspartate (NAA), n-acetylaspartylglutamate (NAAG), Scyllo-Inositol, Glutathione (GSH), Glucose, Taurine, beta-hydroxybutyrate, Cit, Eth, Glycine, PE. 

Additionally, Siemens_7T_steam8_MM also includes nine macromolecules (M0.95, M1.24, M1.43, M1.71, M2.07, M2.30, M3.03, M3.24, M3.98) simulated as detailed in Bell et al. (2024) under review (details and spin systems can be found in https://github.com/HarrisBrainLab/MMSim).

The components of these basis set were simulated using the FID-A script run_simSteamShaped_fast with the parameters detailed below. 

% ************INPUT PARAMETERS**********************************
rfWaveform='asym_exc_minnesota.pta'; %name of RF pulse waveform.
Tp=2.560; %duration of RF pulses[ms]
flipAngle=90;  %Flip Angle of the RF pulses [degrees]
Npts=8210; %number of spectral points
sw=10000; %spectral width [Hz]
Bfield=6.98; %magnetic field strength [Tesla]
%lw=2; %linewidth of the output spectrum [Hz]
thkX=2.5; %slice thickness of x RF pulse [cm]
thkY=2.5; %slice thickness of y RF pulse [cm]
fovX=3.0; %size of the full simulation Field of View in the x-direction [cm]
fovY=3.0; %size of the full simulation Field of View in the y-direction [cm]
nX=32; %Number of grid points to simulate in the x-direction
nY=32; %Number of grid points to simulate in the y-direction
tau1=8; %TE for STEAM sequence [ms]
tau2=40; %TM for STEAM sequence [ms]
centreFreq=2.3; %Centre frequency of simulation [ppm]
% ************END OF INPUT PARAMETERS**********************************

 