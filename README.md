<h1>AtomicESE &ndash; a Neural Network for Evaluation of Solvation Free Energy by Atomic Contributions</h1>
<font face="Open Sans">
<h2>Introduction and User's Guide</h2>

<p><i>AtomicESE</i> is a method for evaluating the <b>solvation free energy</b> &Delta;<i>G°</i><sub>solv</sub> of molecules in organic solvents. 
It is based on a <i>Dense Neural Network</i> and requires only the solute molecular geometry. <i>AtomicESE</i> calculates &Delta;<i>G°</i><sub>solv</sub> by summing atomic contributions, each evaluated by a dense neural network [2]. This atomic network uses 13 physically relevant input features, comprising six local atomic features, two global charge-related molecular properties, and five solvent-specific properties. For neutral solutes, AtomicESE achieves an average RMSE below 0.6 kcal/mol. It also works for ionic solutes.</p>

<p>&Delta;<i>G°</i><sub>solv</sub> can be calculated using the <i>AtomicESE</i> program, 
which can be downloaded free of charge:
<br><a href="https://github.com/vyboishchikov/AtomicESE/blob/main/AtomicESE.exe">AtomicESE.exe</a> &ndash; Windows version;
<br><a href="https://github.com/vyboishchikov/AtomicESE/blob/main/AtomicESE.x">AtomicESE.x</a> &ndash; Linux version;</p>

<p>To run the program from the command line, use the following syntax:</p>
<code>AtomicESE.exe <i>xyz-file</i> -solvent <i>solvent</i> -charge <i>charge</i></code>

<p> The <code>-charge</code> option is optional; the default charge is 0. To print contribution from individual atoms, you may use the <code>-PrintAtomicContributions</code> option</p>

<p><i><b>Warning:</b></i> The <i>xyz-file</i> should contain atomic symbols (or numbers) and Cartesian coordinates (in &#8491;). Do not include any header in the file. An input file example can be found <a href=https://github.com/vyboishchikov/AtomicESE/blob/main/input-example-0423brt.xyz>here</a>.</p>

<p>If you use results calculated by the <i>AtomicESE</i> program, please include at least the following citations:</p>

<ol>
    <li>S. F. Vyboishchikov, <i>AtomicESE program</i>, Girona, <b>2024</b>.</li>
    <li>S. F. Vyboishchikov, <i> J. Comput. Chem.</i>, <b>2025</b>, <i>46</i>, e70104. <a href="https://onlinelibrary.wiley.com/doi/10.1002/jcc.70104">DOI: 10.1002/jcc.70104</a>.</li>
    <li>S. F. Vyboishchikov, <i>Liquids</i>, <b>2024</b>, <i>4</i>, 525&ndash;538. 
    <a href="https://doi.org/10.3390/liquids4030030">DOI: 10.3390/liquids4030030</a></li>
    <li>S. F. Vyboishchikov, <i>J. Chem. Theory Comput.</i>, <b>2023</b>, <i>19</i>, 8340&ndash;8350. 
    <a href="https://doi.org/10.1021/acs.jctc.3c00858">DOI: 10.1021/acs.jctc.3c00858</a></li>
</ol>

<p>Preferably, you may also cite some of our previous related work:</p>

<ol start="5">
    <li>S. F. Vyboishchikov, <i>J. Chem. Inf. Model.</i>, <b>2023</b>, <i>63</i>, 6283&ndash;6292. 
    <a href="https://doi.org/10.1021/acs.jcim.3c00922">DOI: 10.1021/acs.jcim.3c00922</a></li>
    <li>S. F. Vyboishchikov, <i>J. Comput. Chem.</i>, <b>2023</b>, <i>44</i>, 307&ndash;318. 
    <a href="https://doi.org/10.1002/jcc.26894">DOI: 10.1002/jcc.26894</a></li>
    <li>S. F. Vyboishchikov, A. A. Voityuk, <i>Chemical Reactivity, Vol. 2: Approaches and Applications, 
        S. Kaya et al. (Eds.)</i>, Elsevier, <b>2023</b>, 399&ndash;430. 
    <a href="https://doi.org/10.1016/B978-0-32-390259-5.00021-4">DOI: 10.1016/B978-0-32-390259-5.00021-4</a></li>
    <li>S. F. Vyboishchikov, A. A. Voityuk, <a href="https://pubs.acs.org/doi/10.1021/acs.jcim.1c00885">
     <i>J. Chem. Inf. Model., </i><b>2021</b>, <i>61</i></a>, 4544&ndash;4553. DOI: 10.1021/acs.jcim.1c00885</li>
    <li>S. F. Vyboishchikov, A. A. Voityuk, <a href="https://onlinelibrary.wiley.com/doi/abs/10.1002/jcc.26531">
      <i>J. Comput. Chem., </i><b>2021</b>, <i>42</i></a>, 1184&ndash;1194. DOI: 10.1002/jcc.26531</li>
    <li>A. A. Voityuk, S. F. Vyboishchikov,
      <a href="https://pubs.rsc.org/en/content/articlelanding/2020/cp/d0cp02667k">
      <i>Phys. Chem. Chem. Phys.</i> <b>2020</b>, <i>22</i></a>, 14591&ndash;14598. DOI: 10.1039/d0cp02667k</li>
    <li>A. A. Voityuk, S. F. Vyboishchikov, <a href="https://pubs.rsc.org/en/content/articlelanding/2019/cp/c9cp03010g">
    <i>Phys. Chem. Chem. Phys.</i>, <b>2019</b>, <i>21</i></a>, 875&ndash;874. DOI: 10.1039/c9cp03010g</li>
</ol>

<p>For questions related to the <i>AtomicESE</i> method or program, please contact 
<a href="mailto:vyboishchikov@googlemail.com">Sergei Vyboishchikov</a>.</p>
</body>
</html>
