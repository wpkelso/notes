# Pulses
#SignalAnalysis 
[[Signals]] consisting of a single value over a single period of time
$$p(t)=u(t)-u(t-\tau)=
\begin{cases}
1 &\text{, }0\le t\le\tau \\
0 &\text{, else}
\end{cases}
$$

![[pulse.png]]

- One example of a commonly used pulse is the [[Dirac Delta Function]]
- *All pulses can be expressed as a scaled, shifted version of the [[Unit Pulse Function]]*

### Shifting and Scaling
*order of operations does matter, scaling then shifting is different from shifting then scaling*

- First **scale** by $\frac{1}{\tau}$, then **shift** by $t_0$
$$p(\frac{t-t_{0}}{\tau})=
\begin{cases}
1 &\text{, }t_{0}\le t\le\tau \\
0 &\text{, else}
\end{cases}
$$