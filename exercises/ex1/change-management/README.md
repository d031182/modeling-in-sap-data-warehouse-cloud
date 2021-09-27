# Change Management

## The "Tower Problem"
During a modeling and development life cycle, data model changes and modications are just happening. You might want to add addtional fields that you have missed, or delete an outdated one instead. However, when **applying changes to existing data models can be critical, especially if they have dependencies and impact on other models**. This is true for changes that have been applied on the lower stack of the models and eventually the **modeling "tower" starts to wobble and and become very quickly inconsistent**.

<br><br>![](/exercises/ex1/images/cm_01.png)

## Change Management approach in SAP Data Warehouse Cloud
One quick way to stop the **Tower Problem** and inconsistencies is to prohibit and prevent changes and modifications on models with dependencies and impacts on other models.
However, in reality this is not practical. 
1. Strict prevention of inconsistent changes leads very quickly to **modeling inflexiblity**, since changes can not be applied after a model has dependencies. That means, users have to model things from scratch to overcome this strict rule, which is **highly inefficient**.
2. **Changes and modifications can not be always prevented**, e.g. modifications on models in the source system. SAP Data Warehouse Cloud simply has no control over these models and for that can not prohibit such changes. 
