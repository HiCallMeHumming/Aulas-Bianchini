	void Start ()
	{ //movimentar em linha z, distancia 10, sem delay, duracao 2 seg do tipo bounce
		iTween.MoveTo (gameObject,
			iTween.Hash("z", 	 10,
						"delay", 0,
						"time",  2,
				"easetype", iTween.EaseType.bounce));
			}

	//mudar alpha, num tempo de 3 segundos, no tipo pingpong com easeInEaseOut
		iTween.ColorTo (gameObject,
			iTween.Hash ("a", 10,
				"time", 3,
				"looptype", iTween.LoopType.pingPong,
				"easetype", iTween.EaseType.easeInOutCubic));
	}
// mover em um path
		iTween.MoveTo (gameObject,
			iTween.Hash ("path", iTweenPath.GetPath ("S"),
				"time", 10,
				"looptype", iTween.LoopType.pingPong,
				"easetype", iTween.EaseType.easeInOutQuad));
}//shake MT LEGAL PRA FAZER EM JOGOS AONDE UM gameObject TREME!!!
		iTween.ShakePosition (gameObject,
			iTween.Hash (
				"x", 1,
				"y", 1,
				"z", 1,
				"time", 1,
				"delay", 0,
				"looptype", iTween.LoopType.loop));
	}
// vai escalar assim que o Shake terminar (Caso tudo antes dele esteja em //
		public void ScaleTarget() {
				iTween.ScaleTo (target,
				iTween.Hash ("x", 5, "y", 5, "z", 5,"time", 2));
	}

			
