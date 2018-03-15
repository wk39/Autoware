
# Issue List

*  ndt_matching error on repeated run
 
   ```  
        Error: unknown error
        computing/perception/localization/lib/fast_pcl/ndt_gpu/src/MatrixDevice.cu 11
   ```
   -  behavior

      -  after hibernation or sleep mode, ndt_matching is not working...

   -  action

      -  reinstall cuda, cudnn --> __NG__
      -  recompile "autoware", "opencv" --> __NG__
      -  __temporary__ ; 
         undef CUDA_FOUND, USE_FAST_PCL from ndt_matching.cpp, then recompile --> __WORK!__

    
