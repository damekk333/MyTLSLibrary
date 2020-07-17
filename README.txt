1.Import library MyTLSLibrary.jar(configured for all version of Android 1-10) in Android Studio
2.Put cacert, clientcert and clientkey in Assets folder in your app.
3.In app need to be configured three arguments:
        //ca init//
        Certificate ca = new Certificate();
        ca.setCaCertName("cacrt.crt");
        //crt init//
        Certificate crt = new Certificate();
        crt.setCrtCertName("clientcert.crt");
        //key init//
        PrivKey privKey = new PrivKey();
        privKey.setPrivKeyName("clientkey.key");
        //password keystore init//
        PasswordForKeyStore passwordForKeyStore = new PasswordForKeyStore();
        passwordForKeyStore.setPasswordForKeyStore("");
