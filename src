var ap = angular.module("chktable",[]);

ap.directive('ngTableMod',function($timeout){
	return {
		restrict: 'EA',
		link: function(scope,element,attrs){
				$timeout(function(){
					row = [];
					var elementRow = element[0].children[1].children;
					for (var i = 0; i < elementRow.length; i++) {
						row[i] = elementRow[i];
					}
					
					var elementChildren = element[0].children[0].children[0].children;
					
					element.on('click',function(e){
						var order = attrs.ngTableMod;
						var cell = e.target.cellIndex;				
						row.sort(function(a,b){
							if (a.children[cell].innerText > b.children[cell].innerText) {
								if(order=='asc'){
									attrs.ngTableMod = 'desc';
									return 1;
								}
								else{
									attrs.ngTableMod = 'asc';
									return -1;
								}
							}
							if (a.children[cell].innerText < b.children[cell].innerText) {
								if(order=='asc'){
									attrs.ngTableMod = 'desc';
									return -1;
								}
								else{
									attrs.ngTableMod = 'asc';
									return 1;
								}
							}
							return 0;
						});
						
						var tbody = "";
						for(var i=0;i<row.length;i++){
							tbody = tbody + row[i].outerHTML;
						}
						
						element[0].children[1].innerHTML = tbody;
					});
				});
		}
	}
});

ap.controller('table1_con',function($scope){
	
});
