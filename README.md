# Ripple-Effect-Background

Three steps to include a Ripple Effect Background in the application: 

Create a new Java Class: 
       (Code included in the Ripple Background.java)

In the XML Layout: 

       <com.deeplin.synapses.RippleEffect
            android:id="@+id/rippleEffect"
            android:layout_width="0dp"
            android:layout_height="0dp"
            app:layout_constraintBottom_toBottomOf="parent"
            app:layout_constraintEnd_toEndOf="parent"
            app:layout_constraintStart_toStartOf="parent"
            app:layout_constraintTop_toTopOf="parent"
            app:rb_color="@color/base_color"
            app:rb_duration="3000"
            app:rb_radius="32dp"
            app:rb_rippleAmount="4"
            app:rb_scale="6">

            <ImageButton
                android:id="@+id/camera"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_centerInParent="true"
                android:background="@android:color/transparent"
                android:src="@drawable/ic_camera_alt_black_56dp" />
        </com.deeplin.synapses.RippleEffect>
        
In the Main Activity:

         rippleBackground.startRippleAnimation();
