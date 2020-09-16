     private fun loadingAlertDialog() {
            var layoutParams: WindowManager.LayoutParams? = null
            val inflate = View.inflate(FontsApp.instance, R.layout.layer_lock_dialog, null)
            val builder = AlertDialog.Builder(FontsApp.instance, R.style.Translucent_NoTitle)
                    .setView(inflate)
           val create =  builder.create()
    //        inflate.findViewById<View>(R.id.iv_lock_return).setOnClickListener { alertDialog!!.dismiss() }
            inflate.findViewById<View>(R.id.iv_unlock).setOnClickListener {
                create.dismiss()
    
            }
            val windowToken: IBinder? = textViewFlipper?.windowToken
            val window = create.window
            layoutParams = window?.attributes
            layoutParams?.token = windowToken
            layoutParams?.type = 1000
            window?.attributes = layoutParams
            window?.addFlags(WindowManager.LayoutParams.ALPHA_CHANGED)
        if (FontsApp.instance.curActivity is Activity) {
            val activity = FontsApp.instance.curActivity as Activity
            if (!activity.isFinishing) {
                create.show()
            }
        }
    
        }