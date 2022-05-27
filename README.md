# About Domino Engine
Domino Engine is a modified Psych Engine v0.4.2 that adds stuff like icon bounce, watermark, load screen when starting the game and shaders.

# How do I compile?
Look up a tutorial ig idk and USE v4.1.5 SO IT CAN WORK.

# How do I add a funny wavy background like from the hit and very meme mod dave and bambi
Here is the code lmao

                     case 'put your stage here':
			{
				defaultCamZoom = 0.85;
				curStage = 'put your stage here';
				var bg:FlxSprite = new FlxSprite(-600, -200).loadGraphic(Paths.image('put your stage here'));
				bg.antialiasing = true;
				bg.scrollFactor.set(0.6, 0.6);
				bg.active = true;

				add(bg);
				#if windows
				// below code assumes shaders are always enabled which is bad
				var testshader:Shaders.GlitchEffect = new Shaders.GlitchEffect();
				testshader.waveAmplitude = 0.1;
				testshader.waveFrequency = 5;
				testshader.waveSpeed = 2;
				bg.shader = testshader.shader;
				curbg = bg;
				#end
			}
			
ur welcome
