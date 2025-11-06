# Waves in the Ocean

## The Waves that we do not see.

If you stand along the coast of the Mediterranean Sea or the Atlantic Ocean, waves are an obvious feature of the seascape. During stormy days, they cover the ocean surface with white patches extending to the horizon. These waves break both offshore and near the shore, often in plunging patterns when the sand bars are steep. They are likely the type of ocean wave most familiar to humanity, described for centuries in various accounts and literary works — from early testimonies to epics such as The *Odyssey* (8th century BCE). Yet, many other types of waves populate the ocean, some barely visible to the human eye.


##### Rossby Waves

These waves are both atmospheric and oceanic. Let’s focus on those in the ocean. They exist because of the Earth’s sphericity, which causes the Coriolis force to vary with latitude. This latitudinal gradient of the Coriolis parameter acts as the restoring force for these waves. These waves are generated because of an external disturbance of an amount of fluid parcels, displacing them northward or southward. The conservation of  the *absolute vorticity* of the parcels (the amount of intrinsic parcel rotation + the Coriolis-force-induced rotation) induces a westward motion of the water under the form of waves. These low-amplitude planetary waves, with wavelengths of thousands of kilometers, propagate slowly across the ocean. They can be observed from space using satellite-derived sea surface height measurements.

```{figure} /figures/rossby_waves.gif
---
width: 100%
name: rossby_wave
---
Observed equatorial Rossby waves and ENSO-related warm water volume changes in the equatorial Pacific Ocean from Altimetry (Journal: J. Geophys. Res., 113, C06003, doi:10.1029/2007JC004613)
```

 More detail in Chapter 9 of {cite:t}`cushman2011introduction` and {cite:t}`chelton1996global`.
 
 
##### Internal Waves

As their name suggests, these waves propagate within the ocean interior. They are primarily observed using moorings that record seawater temperature. Their wavelength (frequency) depend on their generation mechanism. Internal waves can be generated near the surface by wind forcing (indirectly), by the interaction of tidal currents with the continental slope or seamounts (internal tides), or by the interaction between subsurface currents and topographic features (named lee's waves'). The restoring force for these waves is the ocean’s stratification—that is, the vertical distribution of density in the water column.


```{figure} /figures/internal_waves.png
---
width: 100%
name: internal_wave
---
Temperature data collected offshore Martha Vineyard from the (top) morning survey section and (bottom) afternoon section. The black dots on the left edge of each plot mark the nominal instrument depths, and the thick white line marks the depth where the temperature is 1°C less than the Sea Surface Temperature. The along-track distance increases moving onshore from south to north. (Journal: Farrar, J. T., C. J. Zappa, R. A. Weller, and A. T. Jessup (2007), Sea surface temperature signatures of oceanic internal waves in low winds, J. Geophys. Res., 112, C06014, doi:10.1029/2006JC003947.)
```

Although these waves propagate inside the ocean, they have a surface signature and, therefore, can be visible by satellites.

More details in {cite:t}`leblond1981waves`.

```{figure} /figures/internal_wave_surface.jpg
---
width: 100%
name: internal_wave_surface
---
Optical image from ERS-1 of an internal wave train in the Gilbraltar Strait. Credit ESA.
```


##### Tides (external)

It may seem surprising to say that we cannot see these waves, yet their amplitude varies greatly depending on where we are on Earth. For instance, a regular swimmer in the Mediterranean would hardly notice any change in sea level due to tides, while for a Breton seafarer, tides are a central feature of daily life. From a human perspective, these waves have a period of roughly 12 hours—two high tides and two low tides per day—mainly driven by the gravitational attraction of the Moon. As we will see later in this module, the Moon-induced gravital force on the ocean is not the only source of tidal sea level variations. The propagation of tidal waves is influenced by bathymetry and the Coriolis force. The latter explains why the tidal range along the Normandy coast is much larger than on the opposite side of the English Channel. There are also locations in the ocean where the tidal sea surface height variations are nearly zero. These points, named *amphidromic points*, arise from the combined effects of basin geometry and the Coriolis force. 

```{figure} /figures/tide_amphidromic_points.jpg
---
width: 100%
name: tides
---
Amphidromic points (locations where the heigh different between high and low tide is equal to 0). for the M2 harmonic. Picture credit: R. Ray, TOPEX/Poseidon: Revealing Hidden Tidal Energy GSFC, NASA. Redistribute with credit to R. Ray, as well as NASA-GSFC, NASA-JPL, Scientific Visualization Studio, and Television Production NASA-TV/GSFC
```

More details in {cite:t}`simon2007maree`.
 
##### Other *invisible to the naked eye* waves:
If you are curious about ocean waves you can refer to the following references:
- Inertial waves ({cite:t}`alford2016near`)
- Coastal shelf and trapped waves ({cite:t}`mysak1980recent`)
- Infragravity waves ({cite:t}`bertin2018infragravity`)
- ...

## The Waves that we do see.

In the present module we will mainly focus on what we call surface gravity waves (SGW, waves), basically the waves you see when you go to the coast. 

```{figure} /figures/wave_field_FLIP.png
---
width: 100%
name: FLIP
---
An example of a wave system offshore. (credit: L.Grare)
```

##### Wave Generation
These waves are generated by the wind ({cite:t}phillips1957generation, miles1957generation). However, the processes responsible for the very first ripples produced by a wind gust remain an active area of research. The properties of waves strongly depend on the storm that generated them — including wind speed, the area over which the wind blew, and the duration of the event. If you live near the coast, you have probably noticed how sensitive the ocean surface is to changes in wind conditions.

##### Wave Propagation
The wave propagation properties, such as their phase and group velocity can be described from the wave dispersion relationship. In this module, we will not derive this relationship, but it is an interesting exercise that involves differential fluid mechanics equations (for the curious!).

$$
\omega^2 = gktanh(kD),
$$

with g the acceleration due to the gravity, which acts as the restoring force of the waves, and D the depth below the wave field. From this relation you can compute the wave wavenumber (wavelength) for a given wave frequency (period). However, one can notice that this relationship cannot be inverted i.e., compute k from $\omega$. Fortunately, the $tanh$ function can be approximated based on its argument (kD):
 -  If kD tends toward 1, we are in a shallow water regime and $\omega^2 \sim \sqrt{kD}k$
 -  If kD tends toward a big number, therefore we are in a deep water regime and $\omega^2 \sim gk$. 
- For intermediate water (kD$\sim$ 1), the full expression of the dispersion relationship must be considered, and inverting it requires numerical methods (e.g., the Newton–Raphson method).

```{figure} /figures/approx_dispersion_rel.png
---
width: 100%
name: dispersion_relationship_approximation
---
Functional form of the dispersion relationship in shallow (left) and deep water (right) regime.
```

##### Wave Dissipation

If waves becomes too steep they can break. More specifically, these breakings occurs when the highest orbital velocity (the wave-induced motion of water particles) exceed the phase speed of the waves. It can be due to many different factors. When waves break they create these famous active ocean turbulence at the ocean surface and leave calm foam patches in the lee. Wave breakers and more generally waves play a crucial role in the air-sea Climate system by modulating the exchange of heat, momentum, and matter between the atmosphere and the ocean ({cite:t}`cavaleri2012wind`).

The description of SGW provided in this jupyter book is not exhaustive at all, it represent only the theoretical materials needed for the coming tutorials. I highly recomend to the attendees to make their own literature. Some book to start: ({cite:t}`holthuijsen2010waves,  ardhuin2020ocean, miles1967dynamics`).

To summarize all, these waves can be described with an amplitude, wavelength, direction and phase. Note that the variable used to describe the waves is not necessary the height but can be temperature, current velocity, salinity, pressure, etc. 


