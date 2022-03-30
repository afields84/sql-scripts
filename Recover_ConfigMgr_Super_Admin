/* You use the following commands in conjunction with SSMS to restore or recover the super administrator within your ConfigMgr environment. */

/* Find the user's AdminID */
SELECT * FROM RBAC_Admins

/* Find the user's current role for their default category name */
SELECT * FROM v_SecuredScopePermissions where AdminID = '<Designated User’s AdminID>' and CategoryName = 'Default'

/* Update the CategoryID for the user to SMS00ALL */
UPDATE v_SecuredScopePermissions Set CategoryID = 'SMS00ALL' where AdminID = '<Designated User’s AdminID>' and CategoryName = 'Default'
