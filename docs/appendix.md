# (APPENDIX) Appendix {-} 



# Technical details  {#technical-details}

## Basic information

* STRAF is hosted on an Amazon Web Services (**AWS**) server located in __Ireland__.

* STRAF has __2 CPUs__ and __4 gigabytes of memory__ available on the server. It is 
enough for the vast majority of cases, but might not be enough if your dataset
is too large (too many samples, or too many loci). 

* The web application is based on the __R-Shiny framework__. __R__ is an open source
programming language particularly popular in data science. [Shiny](https://www.rstudio.com/products/shiny/) is an 
open source __R__ package that provides a web framework for building web 
applications using R.

:::{.small}
<div class="figure">
<img src="img/r-logo.png" alt="The R logo." width="100%" />
<p class="caption">(\#fig:r-logo)The R logo.</p>
</div>
:::

## Understanding STRAF's performance

When you open STRAF, a new session starts. When you close your browser or the tab,
the session is closed and your data and computations are deleted.

STRAF can accept an unlimited number of user connections at the same time. 
However, the computational resources are shared between users. In other words,
multiple users can connect at the same time, but computations will be ran one after
the other. If you wait longer than usual for a given task, it is likely
that someone else is using the server. Please keep this in mind and try to avoid
unnecessary computations!

STRAF has limited resources, as described above, and this can be limiting if your
dataset is too large because you have too many samples or loci. In that case,
you could consider trying to run STRAF locally as outlined in __Chapter__ \@ref(local-computer). You could even host it on your own institution's server, in that
case feel free to contact us as we would be happy to help in the process.


## External dependencies

STRAF wouldn't exist without the amazing community of R developers who contributed
great resources and packages.

The application uses several genetics packages:

* `genepop`

* `edegenet`

* `hierfstat`

* `pegas`

More generic data science packages are also used:

* Shiny-related packages: `shiny`, `colourpicker`, `shinycssloaders`, `shinyWidgets`

* The "tidyverse": `dplyr`, `tidyr`, `ggplot2`, `magrittr`, `openxlsx`, `reshape2`, `ggrepel`

# STRAF's commitments {#straf-commitments}

## STRAF will always remain free and open source

STRAF is a __free__ and __open-source__ software. As free software advocates, we believe 
anyone should be able to __run__ the software, __study__ the software, 
__modify__ the software, and to __share__ copies of the software. That is why 
STRAF is licensed under the permissive __GNU General Public License version 3__. 
Here is the [full text of the GPL-3 license](https://www.gnu.org/licenses/gpl-3.0.txt).

For the most curious of you, you can view all the [source code of STRAF on GitHub](https://github.com/agouy/straf).


## STRAF is carbon-neutral

Hosting a web application onto a server requires energy, and energy is becoming
more and more precious. For that reason, STRAF is hosted on a server that is
on a carbon-neutral data center and that will be fully powered by renewable energies by 2025.

This book and STRAF's code source are hosted onto GitHub servers, which are
carbon-neutral as well since 2019.

