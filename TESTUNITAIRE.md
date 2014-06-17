E4-Android
==========

/** Test unitaire à palcer au même niveau que les classes dans un package Test
*/
package com.sio.arbimatch.test;

import android.test.InstrumentationTestCase;

import com.sio.arbimatch.classe.But;
import com.sio.arbimatch.classe.Carton;
import com.sio.arbimatch.classe.Club;
import com.sio.arbimatch.classe.Joueur;
import com.sio.arbimatch.classe.Match;
import com.sio.arbimatch.classe.Remplacement;

import java.util.ArrayList;

/**
 * Created by Litwinczuk on 30/05/14.
 */
public class test_unit extends InstrumentationTestCase {
    public void test() throws Exception {

            Club c3 = new Club(1,"Guillaume");

            Joueur J1C1 = new Joueur(1,"Stan","Smith",true);
            c3.ajouterTitulaire(J1C1);

            if ( c3.getLesTitulaires().size() == 1 ){
                System.out.print("il y a bien un seul joueur");
            }
            else{
                System.out.print("Erreur");
            }

        }
    }

