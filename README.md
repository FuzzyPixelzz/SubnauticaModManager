# shutdown not restart
this branch aims to allow reverting the restart functionality to before commit b21acbd97fc5dd2eb83993e414fa24b1ccd88f17

to that end, a boolean config option will be added to check against

the relevant code can be found at https://github.com/FuzzyPixelzz/SubnauticaModManager/blob/cb0f6bc64e0901c034df5885ab85a0b7fc732dcd/SubnauticaModManager/ModManagerFileArranger/Program.cs#L55
since that appears to be part of a separate module/program, it will probably be required to implicitly load the config file from the bepinex/config directory
