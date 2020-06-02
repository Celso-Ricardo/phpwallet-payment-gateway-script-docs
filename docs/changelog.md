Changelog
=========

##__Version 3.4__

__(06/02/2020)__

1. fixed user impersonation
2. fixed Paystack bug.

__files__
<pre>
	modified:   app/Http/Controllers/PaystackController.php
    modified:   app/Http/Controllers/ProfileController.php
    modified:   resources/views/welcome.blade.php
</pre>


##__Version 3.2__

__(03/30/2020)__

1. added ability to delete expired transactions.
2. fixed email notifications for tickets.
2. added Escrow feature.

__files__
<pre>
	modified:   app/Http/Controllers/AddCreditController.php
	modified:   app/Http/Controllers/DepositController.php
	new file:   app/Http/Controllers/EscrowController.php
	modified:   app/Http/Controllers/HomeController.php
	modified:   app/Http/Controllers/IPNController.php
	modified:   app/Http/Controllers/MoneyTransferController.php
	modified:   app/Http/Controllers/TransactionController.php
	modified:   app/Http/Controllers/WithdrawalController.php
	new file:   app/Mail/Deposit/depositCompletedUserNotificationEmail.php
	new file:   app/Mail/Deposit/depositRequestAdminNotificationEmail.php
	renamed:    app/Mail/depositRequestUserEmail.php -> app/Mail/Deposit/depositRequestUserEmail.php
	new file:   app/Mail/Withdrawal/withdrawalCompletedUserNotificationEmail.php
	new file:   app/Mail/Withdrawal/withdrawalRequestAdminNotificationEmail.php
	new file:   app/Mail/Withdrawal/withdrawalRequestUserEmail.php
	deleted:    app/Mail/depositEmail.php
	modified:   app/Mailers/AppMailer.php
	new file:   app/Models/Escrow.php
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
	new file:   resources/views/escrow/escrow_agreement.blade.php
	new file:   resources/views/escrow/form.blade.php
	modified:   resources/views/home/partials/transactions_to_confirm.blade.php
	modified:   resources/views/layouts/aside.blade.php
	modified:   resources/views/partials/sidebar.blade.php
	modified:   resources/views/sendmoney/index.blade.php
	new file:   resources/views/vendor/voyager/escrows/browse.blade.php
	modified:   resources/views/vendor/voyager/withdrawals/edit-add.blade.php
	modified:   resources/views/withdrawals/withdrawalRequestForm.blade.php
	modified:   routes/web.php
</pre>


##__Version 3.1__

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