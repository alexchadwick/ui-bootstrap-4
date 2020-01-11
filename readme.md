# UI BOOTSTRAP 4

**UI Bootstrap 4 Custom Build**

### Usage

```javascript
import uiBootstrapModule from './ui-bootstrap-4/ui-bootstrap-custom-tpls-3.0.6.js';

 var modalInstance = $uibModal.open({
            animation: true,
            ariaLabelledBy: 'modal-title',
            ariaDescribedBy: 'modal-body',
            template: require('./_modals/modal.tpl.html'),
            controller: 'ModalController',
            controllerAs: '$ctrl',
            size: 'lg',
            resolve: {
                location: function(appService) {
                    return appService.getOrganizationLocation(organization_id, location_id)
                        .then(function (res) {
                            return res.data;
                        })
                },
               
            }
        });
        return modalInstance;
```



### Support
Support Bootstrap Modals

### Notes

Original Project:
 - ui-bootstrap4
    - http://morgul.github.io/ui-bootstrap4/