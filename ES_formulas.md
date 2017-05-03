In ALEX we have four basic photon streams: 
\(F_{DexDem}, F_{DexAem}, F_{AexDem}, F_{AexAem}\).
The \(F_{AexDem}\) stream only contains background 
because there is no fluorescent emission in the D
spectral band during A-laser excitation.
For simplicity, we assume here and in the following that all
the quantities are corrected for background.

In PAX, there is a period with only D excitation
that we denote as \(D_{ex}\), and a period with both D and A
excitations that we call \(DA_{ex}\).
With this convention, we can name the four photon stream in PAX
simply replacing \(A_{ex}\) with \(DA_{ex}\):
\(F_{DexDem}, F_{DexAem}, F_{DAexDem}, F_{DAexAem}\).
Note however that \(F_{DAexDem}\) in PAX contains
fluorescent signal because of the D laser excitation.
With this notation we can define the total signal during 
D excitation (burst size):

\[
\Lambda_R = {F_{DexDem} + F_{FRET}}
\label{eq:burstsize_raw}
\]

\[
\Lambda = {\gamma\,F_{DexDem} + F_{FRET}}
\label{eq:burstsize}
\]

where \(F_{FRET}\) is equal to \(F_{DexAem}\) after
D-leakage and A-direct-excitation corrections:

\[
F_{FRET} = F_{DexAem} - Lk\,F_{DexDem} - Dir
\label{eq:F_FRET}
\]

With this definition we can write
\[
E = \frac{F_{FRET}}{\gamma\,F_{DexDem} + F_{FRET}}
\label{eq:E}
\]

\[
E_{PR} = \frac{F_{FRET}}{\gamma\,F_{DexDem} + F_{FRET}}
\label{eq:Epr}
\]


Eq. \ref{eq:E} is exactly the same for both ALEX and PAX.
Conversely, the stoichiometry \(S\) is slightly different
in the two cases. In ALEX we define \(S\) as:

\[
S = \frac{F_{FRET} + F_{DexDem}}{F_{FRET} + F_{DexDem} + F_{AexAem}}
\label{eq:S}
\]

and the corrected version \(S_{\gamma\beta}\) as:

\[
S_{\gamma\beta} = \frac{F_{FRET} + \gamma F_{DexDem}}
{F_{FRET} + \gamma F_{DexDem} + F_{AexAem}/\beta}
\label{eq:Sgb}
\]

In PAX, we do not measure the \(F_{AexAem}\) stream, but we can compute it as:

\[
\tilde{F}_{AexAem} = F_{DAexAem} - F_{DexAem}
\label{eq:pax_Faa}
\]

With definition of eq. \ref{eq:pax_Faa} the expressions for \(S\) 
and \(S_{\gamma\beta}\) become formally identical to eq. \ref{eq:S} 
and \ref{eq:Sgb} were the only difference is replacing 
\(F_{AexAem}\) with \(\tilde{F}_{AexAem}\):

\[
S = \frac{F_{FRET} + F_{DexDem}}
{F_{FRET} + F_{DexDem} + \tilde{F}_{AexAem}}
\label{eq:S}
\]

\[
S_{\gamma\beta} = \frac{F_{FRET} + \gamma F_{DexDem}}
{F_{FRET} + \gamma F_{DexDem} + \tilde{F}_{AexAem}/\beta}
\label{eq:Sgb}
\]

In PAX we can take advantage of the additional signal in \(F_{AexDem}\)
and derive an equivalent set of PAX enahanced expressions for \(E\)
and \(S\). In particular, we can replace  \(F_{DexDem}\) with
\(F_{DexDem} + F_{AexDem}\) and \(F_{DexAem}\) with \(2\,F_{DexAem}\).

\[
E_{PAX} = \frac{2\,F_{FRET}}
{\gamma\,(F_{DexDem} + F_{AexDem}) + 2\,F_{FRET}}
\label{eq:Epax}
\]

\[
S = \frac{F_{DexAem} + F_{DexDem}}{F_{DexAem} + F_{DexDem} + \tilde{F}_{AexAem}}
\label{eq:S}
\]

\[
S_{\gamma\beta,PAX} = \frac{2 F_{FRET} + \gamma\,(F_{DexDem} + F_{AexDem})}
{2 F_{FRET} + \gamma\,(F_{DexDem} + F_{AexDem}) + 2\tilde{F}_{AexAem}/\beta}
\label{eq:Sgb}
\]