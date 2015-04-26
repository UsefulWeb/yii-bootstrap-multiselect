# yii-bootstrap-multiselect
Simple asset for davidstutz/bootstrap-multiselect

Example :

```
<?php 
  
    $this->widget('path.to.plugin',array(
      // 'name' or 'attribute' and 'model'
      'name' => $name, 
      'value' => $model->value, 
      // availiable options
      'data' => $data,
      'htmlOptions' => array(
        'class' => 'col-sm-5 form-control',
        // if you need multiple
        'multiple' => true,
      ),
      'pluginOptions' => array(
        // part of plugin options, you can see all at https://github.com/davidstutz/bootstrap-multiselect
        'filterPlaceholder' => 'Поиск',
        'maxHeight' => 300,
        'enableFiltering' => true,
        'includeFilterClearBtn' => true,
        'includeSelectAllOption' => true,
        'selectAllText' => 'Clear all',
        'allSelectedText' => 'All items have been selected',
        'nonSelectedText' => 'Select items',
        'templates' => array(
          'filter' => '<li class="multiselect-item filter"><div class="input-group"><span class="input-group-addon"><i class="fa fa-search"></i></span><input class="form-control multiselect-search" type="text"></div></li>',
          'filterClearBtn' => '<span class="input-group-btn"><button class="btn btn-default multiselect-clear-filter form-control" type="button"><i class="fa fa-remove"></i></button></span>',
        )
      ),
    ));
  ?>
```
