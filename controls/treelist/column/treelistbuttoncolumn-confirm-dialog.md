---
title: TreeListButtonColumn Confirm Dialog
page_title: TreeListButtonColumn Confirm Dialog | UI for ASP.NET AJAX Documentation
description: TreeListButtonColumn Confirm Dialog
slug: treelist/column/treelistbuttoncolumn-confirm-dialog
tags: treelistbuttoncolumn,confirm,dialog
published: True
position: 4
---

# TreeListButtonColumn Confirm Dialog



The native button column of RadTreeList allows for the display of a confirmation dialog before the column command is fired.

## Confirm Message

The confirmation message is set through the __ConfirmText__ property of the button column. Going a bit furtheryou can customize the message including in it information from various fields present in the data the tree list is bound to. The fields which values should go into the confirmation message are defined in the __ConfirmTextFields__property that accepts a string array. Then you should set the __ConfirmTextFormatString__ where each placeholder will correspond to a field in the ConfirmTextFields on a ascendingly-ordered sequence basis. For example, if you have an edit button columnwith __ConfirmTextFields = “BookID, Title”__ and __ConfirmTextFormatString = “Edit information for book with ID = {0}, titled {1}?”__ and there comes a BookID = 1 and Title = “Mount Athos” for the first record, you will get a confirmation dialog of __“Edit information for book with ID = 1, titled Mount Athos?”__

## Confirmation Dialog Type

The confirmation dialog can be either a classic alert window or a RadWindow control. This preference is indicated through the __ConfirmDialogType__ property. If the RadWindow type is chosen, there must be a RadWindowManager added to the page otherwise the column will resort to using the default classic confirmation window.

## Confirmation Dialog Customization

In addition, if you choose to use the RadWindow confirmation dialog you can additionally customize it by setting its height and width through the __ConfirmDialogHeight__ and __ConfirmDialogWidth__ properties respectively and assign a window title using the __ConfirmTitle__ property.