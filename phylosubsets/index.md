---
layout: default
title: Phylogeny subsets
weight: 5
---



Phylogeny subsets
=================


This tool provides a simple way to produce distributions of trees with subsets
of taxa. If larger subsets are required you can [download full trees](https://data.vertlife.org/).

The tool first trims to a subset, and then samples trees from a chosen
pseudo-posterior distribution. *Note that any further analyses should only
be conducted with a large sample of trees.*

**Instructions**

1. Select species from the list which follows the taxonomy. Then copy and paste or drag and drop
them into the box to the right. 
  - _Alternatively_, download the [taxonomy file](https://data.vertlife.org/vertlife_taxonomies.csv) for your group
and paste species names from the "Scientific" column.  
		* Link to the [direct data download page](https://data.vertlife.org), including full tree sets and higher-level taxonomy in some cases (e.g., for [Mammals](https://data.vertlife.org/mammaltree/taxonomy_mamPhy_5911species.csv) and [Birds](https://data.vertlife.org/birdtree/BLIOCPhyloMasterTax.csv))
  - _Please note_: If you have different names, you will have to resolve to the available list. 
2. Choose a tree distribution (see paper for details).  
3. Select the number of trees to download (defaults to minimum of 100)  
4. Click "Get Trees" to download a zipped set of randomly selected
trees with metadata including accession numbers and citations to original  
sources.  
5. __Please wait a minute then check the job status using your email address and job ID. If the download is complete, then you can download the trees. If the trees are not ready, please wait another minute and check the status again.__

<div class="well well-sm">
  <p>
    <strong>Results taking longer than expected? </strong>
    <br />Traffic volume may result in longer processing times. If you don't recieve an email with the completed subset trees within 24 hours, please <a href="mailto:support@vertlife.org">contact us</a>.
  </p>
</div>

<div class="container well well-lg">
  <div class="row">
    <form class="col-md-9">
      <div class="form-group">
        <label>Select Group: </label> &nbsp; &nbsp; 
          <label class="radio-inline">
            <input type="radio" name="grpTaxa" id="grpTaxaAmph" value="amphibiantree" checked> Amphibians
          </label>
          <label class="radio-inline">
            <input type="radio" name="grpTaxa" id="grpTaxaBird" value="birdtree"> Birds
          </label>
          <label class="radio-inline">
            <input type="radio" name="grpTaxa" id="grpTaxaMammal" value="mammaltree"> Mammals
          </label>
          <label class="radio-inline">
            <input type="radio" name="grpTaxa" id="grpTaxaShark" value="sharktree"> Sharks
          </label>
          <label class="radio-inline">
            <input type="radio" name="grpTaxa" id="grpTaxaSqam" value="squamatetree"> Squamates
          </label>
      </div>
      <hr />
      <div class="form-group">
        <label>Select from the following <span id="baseTreeName"></span>: </label>
        <div class="row">
          <div class="speciesContainer col-md-5"></div>
          <div class="selectedContainer col-md-5">
            <textarea id="selected" placeholder="Paste species names here (one binomial per line)."></textarea>
          </div>
        </div>
      </div>
    </form>
  </div>
  <div class="row">
    <form class="form-horizontal col-md-9">
      <div class="form-group">
        <label for="email" class="col-sm-5 control-label">Please provide your email address: </label>
        <div class="col-sm-7">
          <input type="text" class="form-control input-sm" name="email" id="email">
          <p class="help-block"><em><strong>Note:</strong> Once completed, a link to the generated phylogeny subsets will be emailed to the address provided.</em></p>
        </div>
      </div>
      <div class="form-group">
        <label for="treeset" class="col-sm-5 control-label">Source of trees: </label>
        <div class="col-sm-7">
          <select name="treeset" id="treeset" class="form-control input-sm"></select>
        </div>
      </div>
      <div class="form-group">
        <label for="treenum" class="col-sm-5 control-label">Select number of trees to create: </label>
        <div class="col-sm-7">
          <input id="treenum" type="text" size="2" class="form-control input-sm" value="100">
          <p class="help-block"><em><strong>Note:</strong> We need a minimum of <strong><span id="tsmin">100</span></strong> and a maximum <strong><span id="tsmax">10,000</span></strong></em></p>
        </div>
      </div>
      <div class="form-group">
        <div class="col-sm-5">&nbsp;</div>
        <div class="col-sm-7">
          <button type="button" class="btn btn-default btn-sm" id="btnGetTrees">Get Trees</button>
          <span><img id="loading" src="/images/loading.gif" onload="$(this).toggle(false)" style="display: none;" /></span>
        </div>
      </div>
      <div id="status" class="form-group"></div>
    </form>
  </div>
  <hr />
  <h4>Check the status of your job request here</h4>
  <div>
    <div class="row">
      <div class="col-xs-4">
        <label for="emailStatus">Email address: </label>
        <input type="text" class="form-control input-sm" name="emailStatus" id="emailStatus" value="">
      </div>
      <div class="col-xs-5">
        <label for="jobid">Job ID: </label>
        <input type="text" class="form-control input-sm" name="jobid" id="jobid" value="">
        <p class="help-block">e.g. tree-pruner-ade65c04-65fc-4028-a2bb-8da4d560bb97</p>
      </div>
      <div class="col-xs-3">
        <div>&nbsp;</div>
        <button type="button" class="btn btn-default btn-sm" id="btnStatus">Check Status</button>
        <span><img id="loadingCheck" src="/images/loading.gif" onload="$(this).toggle(false)" style="display: none;" /></span>
      </div>
    </div>
    <div id="statusCheck" class="col-md-9"></div>
  </div>
</div>
<script src="/js/subsets.js"></script>