Changelog
=========

##__Version 2.9__

__(03/27/2020)__

1. added admin email notification for new deposit requests
2. added admin user notification for deposit requests waiting to be reviewed
3. added admin user notification for completed deposits
4. added admin email notification for new withdrawal requests
5. added admin user notification for withdrawal requests waiting to be reviewed
6. added admin user notification for completed withdrawal
7. improved the withdrawal flow for admins
8. improved the currency exchange flow for regular users
9. improved the update exchange rate flow for admins 

__files__
<pre>
		modified:   app/Http/Controllers/AddCreditController.php
		modified:   app/Http/Controllers/DepositController.php
		modified:   app/Http/Controllers/WithdrawalController.php
		new file:   app/Mail/Deposit/depositCompletedUserNotificationEmail.php
		new file:   app/Mail/Deposit/depositRequestAdminNotificationEmail.php
		renamed:    app/Mail/depositRequestUserEmail.php -> app/Mail/Deposit/depositRequestUserEmail.php
		new file:   app/Mail/Withdrawal/withdrawalCompletedUserNotificationEmail.php
		new file:   app/Mail/Withdrawal/withdrawalRequestAdminNotificationEmail.php
		new file:   app/Mail/Withdrawal/withdrawalRequestUserEmail.php
		deleted:    app/Mail/depositEmail.php
		modified:   app/Models/Withdrawal.php
		modified:   resources/views/deposits/addCreditForm.blade.php
		new file:   resources/views/email/deposit/depositCompletedUserNotificationEmail.blade.php
		new file:   resources/views/email/deposit/depositRequestAdminNotificationEmail.blade.php
		new file:   resources/views/email/deposit/depositRequestUserEmail.blade.php
		deleted:    resources/views/email/depositCompleted.blade.php
		deleted:    resources/views/email/depositRequestAdminEmail.blade.php
		deleted:    resources/views/email/depositRequestUserEmail.blade.php
		new file:   resources/views/email/withdrawal/withdrawalCompletedUserNotificationEmail.blade.php
		new file:   resources/views/email/withdrawal/withdrawalRequestAdminNotificationEmail.blade.php
		new file:   resources/views/email/withdrawal/withdrawalRequestUserEmail.blade.php
		modified:   resources/views/partials/sidebar.blade.php
		modified:   resources/views/vendor/voyager/withdrawals/edit-add.blade.php
		modified:   resources/views/withdrawals/withdrawalRequestForm.blade.php
</pre>