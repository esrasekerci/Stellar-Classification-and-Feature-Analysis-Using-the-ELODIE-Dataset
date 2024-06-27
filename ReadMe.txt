Excerpts from original ReadMe:

III/251             ELODIE library V3.1         (Prugniel+ 2007)
================================================================================
New release of the ELODIE library: Version 3.1
     Prugniel P., Soubiran C, Koleva M., Le Borgne D.
    <astro-ph/0703658 (2007)>
    =astro-ph/0703658
================================================================================
ADC_Keywords: Spectrophotometry ; Atlases ; Spectroscopy ; Populations, stellar
Keywords: atlases - stars: abundances - stars: atmospheres -
          stars: fundamental parameters - galaxies: stellar content

Description:
    ELODIE.3.1 is an updated release of the library published in Prugniel
    & Soubiran (2001A&A...369.1048P, Cat. III/218; and 2004 version, in
    astro-ph/0409214). The library includes 1892* stellar parameters of 
    1353* stars obtained with the ELODIE spectrograph at the Observatoire de
    Haute-Provence 193cm telescope in the wavelength range 390 to 680 nm.
    It provides a wide coverage of atmospheric parameters: Teff from
    3100K to 50000K, logg from -0.25 to 4.9 and [Fe/H] from -3 to +1.
    ...

* Originally 1959 observations of 1388 stars. 
Binary star systems and exotic classes were removed
to streamline the classification task.

================================================================================

Description of file: elodiev2.csv (not an official expansion)

Stellar parameters:
--------------------------------------------------------------------------------
  Units    Label     Explanations
--------------------------------------------------------------------------------
  ---      name      Object identifier
  km/s     vr        Heliocentric radial velocity
  K        teff      Effective temperature
  [cm/s+2] logg      decimal log of surface gravity
  [Sun]    feh       Iron abundance relative to solar
  0.1nm    ca4227    Ca4227 index
  0.1nm    g4300     G4300 index
  0.1nm    hgamA     H gamma A index
  0.1nm    hgamF     H gamma F index
  0.1nm    fe4383    Fe4383 index
  0.1nm    ca4455    Ca4455 index
  0.1nm    fe4531    Fe4531 index
  0.1nm    fe4668    Fe4668 index
  0.1nm    hbeta     Hbeta index
  0.1nm    fe5015    Fe5015 index
  mag      mg1       Mg1 index
  mag      mg2       Mg2 index
  0.1nm    mgb       Mgb index
  0.1nm    fe5270    Fe5270 index
  0.1nm    fe5335    Fe5335 index
  0.1nm    fe5406    Fe5406 index
  0.1nm    fe5709    Fe5709 index
  0.1nm    fe5782    Fe5782 index
  0.1nm    nad       NaD index
  mag      tio1      TiO1 index
  mag      tio2      TiO2 index
  ---      sp_type   Morgan-Keenan Spectral type
  ---      spec     *Main spectral type (Target)

Observation quality parameters:
--------------------------------------------------------------------------------
  Units    Label     Explanations
--------------------------------------------------------------------------------
  ---    q_sp_type  *[A-E] Quality flag on SpType
  ---    q_logg     *[-1,1] Quality flag on logg
  ---    q_feh      *[-1,4] Quality flag on [Fe/H]
  ---    q_vr       *[-1,0] Quality flag on Vr
  [cm/s+2] loggM     Estimated log of surface gravity
  [Sun]    [Fe/H]M   Estimated [Fe/H]

Note on spec:
    Follows the sequence: O, B, A, F, G, K and M. These labels are
    ordinal in nature.

Note on q_sp_type:
    Quality varies from A (well established) to E (not precise).
    Spectral types were queried from an external database. If a star
    was referenced in the literature multiple times with the same
    spectral type, its label received the quality rating A. If a star 
    was only referenced in literature once, and was not observed for 
    long enough for full classification, its label received the
    quality rating E.

Note on q_logg: (see section 2 of paper)
     -- q_logg=1 means that the determination of log.g is taken
        from the literature
     -- q_logg=0 means that log.g was converted from the V absolute
        magnitude from Hiparcos and Teff, using a bolometric correction
        valid for a main sequence start and an empirical mass-to-light
        relation.
     -- q_logg=-1 means an internal determination of the surface gravity

Note on q_feh: (see section 2 of paper)
     -- values from 1 (poor determination) to 4 (excellent)
     -- q_feh=-1 means an internal determination of [Fe/H]

Note on q_vr: (see section 2 of paper)
     -- q_vr = 0 means that vr was estimated from the doppler shift
       measured from a good fit of spectral line profiles
     -- q_vr = -1 means that the fit of spectral lines failed

...

================================================================================
(End)               Philippe Prugniel,  Francois Ochsenbein [CDS]    12-Apr-2007