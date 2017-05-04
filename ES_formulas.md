In ALEX we have two alternation periods \(D_{ex}\)
and \(A_{ex}\) (respectively D or A excitation) and 
four basic photon streams: 
\(F_{DexDem}, F_{DexAem}, F_{AexDem}, F_{AexAem}\).
The \(F_{AexDem}\) stream only contains background 
because there is no fluorescent emission in the D
spectral band during A-laser excitation.
For simplicity, we assume here and in the following that all
the quantities are corrected for background\cite{Ingargiola_2016}.

In PAX, like in ALEX, we have two alternation periods
\(D_{ex}\)
and \(DA_{ex}\): D excitation and D+A excittion the two periods are referred as as \(D_{ex}\)
for the one with D excitation
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
\Lambda = {F_{DexDem} + F_{FRET}}
\label{eq:burstsize_raw}
\]

\[
\Lambda_\gamma = {\gamma\,F_{DexDem} + F_{FRET}}
\label{eq:burstsize}
\]

where \(F_{FRET}\) is equal to \(F_{DexAem}\) after
D-leakage and A-direct-excitation corrections:

\[
F_{FRET} = F_{DexAem} - Lk\,F_{DexDem} - Dir
\label{eq:F_FRET}
\]

With this definition we can write expression for \(E\):

\[
E_{PR} = \frac{F_{FRET}}{\Lambda}
\label{eq:Epr}
\]

\[
E = \frac{F_{FRET}}{\Lambda_\gamma}
\label{eq:E}
\]


Eq. \ref{eq:E} is exactly the same for both ALEX and PAX.
Conversely, the stoichiometry \(S\) is slightly different
in the two cases. In ALEX we define \(S\) as:

\[
S = \frac{\Lambda}{\Lambda + F_{AexAem}}
\label{eq:S}
\]

and the corrected version \(S_{\gamma\beta}\) as:

\[
S_{\gamma\beta} = \frac{\Lambda_\gamma}
{\Lambda_\gamma + F_{AexAem}/\beta}
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
S = \frac{\Lambda}
{\Lambda + \tilde{F}_{AexAem}}
\label{eq:Spax}
\]

\[
S_{\gamma\beta} = \frac{\Lambda_\gamma}
{\Lambda_\gamma + \tilde{F}_{AexAem}/\beta}
\label{eq:Sgb_pax}
\]

In PAX we can take advantage of the additional signal in \(F_{AexDem}\)
and derive an equivalent set of PAX enahanced expressions for \(E\)
and \(S\). In particular, we can start defining a PAX-enhanced
D-excitation signal (burst size):

\[
\Lambda_{PAX} = {F_{DexDem} + F_{AexDem} + 2 F_{FRET}}
\label{eq:burstsize_raw_paxe}
\]

\[
\Lambda_{\gamma,PAX} = {\gamma\,(F_{DexDem} + F_{AexDem}) + 2 F_{FRET}}
\label{eq:burstsize_paxe}
\]

With this the expression for \(E\) and \(S\) become:

\[
E_{PR,PAX} = \frac{2\,F_{FRET}}
{\Lambda_{PAX}}
\label{eq:Epr_paxe}
\]

\[
E_{PAX} = \frac{2\,F_{FRET}}
{\Lambda_{\gamma,PAX}}
\label{eq:Epaxe}
\]

\[
S = \frac{\Lambda_{PAX}}
{\Lambda_{PAX} + \tilde{F}_{AexAem}}
\label{eq:Spaxe}
\]

\[
S_{\Lambda_{\gamma,PAX}} = \frac{\Lambda_{\gamma,PAX}}
{\Lambda_{\gamma,PAX} + 2\tilde{F}_{AexAem}/\beta}
\label{eq:Sgb_paxe}
\]
