domain_civicrm
==============

alpha module for creating civicrm domains


global $_domain;

if (!empty($_domain['subdomain'] )) {
switch ($_domain['subdomain']){
case 'bats.fuzion.co.nz' :
define( 'CIVICRM_DOMAIN_ID' , 2 );
define( 'CIVICRM_DOMAIN_GROUP_ID',4 );
define( 'CIVICRM_DOMAIN_ORG_ID' , 74958 );
define( 'CIVICRM_UF_BASEURL' , 'http://bats.fuzion.co.nz/' );
break;
case 'cats.fuzion.co.nz' :
case 'mice.fuzion.co.nz' :
define( 'CIVICRM_DOMAIN_ID' , 3 );
define( 'CIVICRM_DOMAIN_GROUP_ID',5 );
define( 'CIVICRM_DOMAIN_ORG_ID' , 74959 );
define( 'CIVICRM_UF_BASEURL' , 'http://cats.fuzion.co.nz/' );
break;
default :
define( 'CIVICRM_DOMAIN_ID'      , 1 );
define( 'CIVICRM_DOMAIN_GROUP_ID', null );
define( 'CIVICRM_DOMAIN_ORG_ID'  , null );
define( 'CIVICRM_UF_BASEURL'      , 'http://fuzion.co.nz/' );
}
}