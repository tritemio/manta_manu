In ALEX we have two alternation periods \(D_{ex}\)
and \(A_{ex}\) (respectively D or A excitation) and 
two (D and A) detectors. This results in four basic photon streams 
named \(F_{DexDem}, F_{DexAem}, F_{AexDem}, F_{AexAem}\).
The \(F_{AexDem}\) stream only contains background 
because there is no fluorescent emission in the D
spectral band during A-laser excitation.
For simplicity, we assume here and in the following that all
the quantities are corrected for background\cite{Ingargiola_2016}.

Similarly to ALEX, in PAX we have two (D and A) detectors and
two laser alternation periods \(D_{ex}\) and \(DA_{ex}\) denoting,
respectively, D and D+A excitations.
As in ALEX, combining the two excitation periods and the two detectors,
we obtain four basic PAX photon streams named
\(F_{DexDem}, F_{DexAem}, F_{DAexDem}, F_{DAexAem}\).
Formally, the only difference with the ALEX photon stream is that 
\(A_{ex}\) in ALEX is replaced with \(DA_{ex}\) in PAX.
Note however that, in PAX, \(F_{DAexDem}\) contains
fluorescent signal due to D laser excitation.
With this notation, in both ALEX and PAX, we can define 
the total signal during D excitation (e.g. burst size):

\[
\Lambda = {F_{DexDem} + F_{FRET}}
\label{eq:burstsize_raw}
\]

and the \(\gamma\) corrected version\cite{Lee_2005,Ingargiola_2016,Ingargiola_2017}:

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

With this definitions, we can write the proximity ratio \(E_{PR}\) and FRET efficiency \(E\) expression (valid for both ALEX and PAX):

\[
E_{PR} = \frac{F_{FRET}}{\Lambda}
\label{eq:Epr}
\]

\[
E = \frac{F_{FRET}}{\Lambda_\gamma}
\label{eq:E}
\]


While eq. \ref{eq:Epr} and \ref{eq:E} are exactly the same for both ALEX and PAX,
the stoichiometry \(S\) expression is slightly different. 
In ALEX we define \(S\) as:

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

Using eq. \ref{eq:pax_Faa}, the expressions for \(S\) 
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
and derive an equivalent set of "PAX-enahanced" expressions for \(E\)
and \(S\). We can start extending the definitions of the total FRET signal 
of eq. \ref{eq:burstsize_raw} and \ref{eq:burstsize}
by including \(F_{AexDem}\) as follows:

\[
\Lambda_{PAX} = {F_{DexDem} + F_{AexDem} + 2 F_{FRET}}
\label{eq:burstsizerawpaxe}
\]

\[
\Lambda_{\gamma,PAX} = {\gamma\,(F_{DexDem} + F_{AexDem}) + 2 F_{FRET}}
\label{eq:burstsize_paxe}
\]

Based on eq.\ref{eq:burstsizerawpaxe} and \ref{eq:burstsize_paxe}, 
we can write PAX-enhanced expressions for \(E\) and \(S\):

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

Since eq.\ref{eq:Epr_paxe,eq:Epaxe}, 