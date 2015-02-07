# Magento PhpStorm Live Templates

##Installation
Copy the desired live template group file to your PhpStorm live template directory.

###OSX
Copy to ```~/Library/Preferences/WebIde<version number>/templates/``` and reload PhpStorm.

###Linux
Copy to ```~/.WebIDE<version number>/config/templates/``` and reload PhpStorm.

###Windows
Copy to ```<your home directory>\.<product name><version number>\config\templates\``` and reload PhpStorm.

Available templates are:

##Magento XML
| Tab Trigger | Output |
| :--------------- | :-----|
| m:action | ```<action method="$action$">$key$</action>``` |
| m:addCss | ```<action method="addCss"><name>$name$</name></action>``` |
| m:addCssIe | ```<action method="addCssIe"><name>$name$</name></action>``` |
| m:addItem | ```<action method="addItem"><type>$type$</type><name>$name$</name></action>``` |
| m:addJs | ```<action method="addJs"><name>$name$</name></action>``` |
| m:addJsIe | ```<action method="addJsIe"><name>$name$</name></action>``` |
| m:addLinkRel | ```<action method="addLinkRel"><rel>$rel$</rel><href>$href$</href></action>``` |
| m:block | ```<block type="$type$" name="$name$">$end$</block>``` |
| m:block/ | ```<block type="$type$" name="$name$" template="$template$" />``` |
| m:cdata | ```<block type="core/text" name="$name$"><action method="setText"><text><![CDATA[$data$]]></text></action></block>``` |
| m:cms/block | ```<block type="cms/block" name="$name$"><action method="setBlockId"><id>$id$</id></action></block>``` |
| m:core/template | ```<block type="core/template" name="$name$" template="$template$" />``` |
| m:insert | ```<action method="insert"><name>$name$</name></action>``` |
| m:layout | ```<?xml version="1.0"?><layout><default></default></layout>``` |
| m:reference | ```<reference name="$name$">$end$</reference>``` |
| m:remove | ```<remove name="$name$" />``` |
| m:removeItem | ```<action method="removeItem"><type>$type$</type><name>$name$</name></action>``` |
| m:setData | ```<action method="setData"><name>$name$</name><value>$value$</value></action>``` |
| m:setTemplate | ```<action method="setTemplate"><template>$template$</template></action>``` |
| m:unset | ```<action method="unsetChild"><name>$name$</name></action>``` |
| m:unsetData | ```<action method="unsetData">$key$</action>``` |
| m:update | ```<update handle="$handle$" />``` |

##Magento Template
| Tab Trigger | Output |
| :--------------- | :-----|
| m:__ | ```<?php echo $this->__('$string$'); ?>``` |
| m:child | ```<?php echo $this->getChildHtml('$child$'); ?>``` |
| m:getConfig | ```<?php echo Mage::getStoreConfig('$path$'); ?>``` |
| m:globalMessages | ```Mage::getSingleton('core/session')->addNotice('Notice message'); Mage::getSingleton('core/session')->addSuccess('Success message'); Mage::getSingleton('core/session')->addError('Error message');``` |
| m:helper | ```$var$ = Mage::helper('$helper$');``` |
| m:log | ```Mage::log(sprintf("%s", $log$), Zend_Log::DEBUG, '$logfile$.log', true);``` |
| m:logHandles | ```Mage::log(sprintf("Handles: %s", print_r(Mage::app()->getLayout()->getUpdate()->getHandles(), true)), Zend_Log::DEBUG, '$logfile$.log', true);``` |
| m:model | ```$var$ = Mage::getModel('$model$');``` |
| m:skinUrl | ```<?php echo $this->getSkinUrl('$skinUrl$') ?>``` |
| m:url | ```<?php echo $this->getUrl('$url$') ?>``` |