# Augmented_PINNs_-APINNs-



In this paper, we propose the augmented physics-informed neural network (APINN), which adopts soft and trainable domain decomposition and 
flexible parameter sharing to further improve the extended PINN (XPINN) as well as the vanilla PINN methods. In particular, a trainable gate
network is employed to mimic the hard decomposition of XPINN, which can be flexibly fine-tuned for discovering a potentially better partition.
It weight-averages several sub-nets as the output of APINN. APINN does not require complex interface conditions, and its sub-nets can take 
advantage of all training samples rather than just part of the training data in their subdomains. Lastly, each sub-net shares part of the common
parameters to capture the similar components in each decomposed function. Furthermore, following the PINN generalization theory in 
Hu et al. [2021], we show that APINN can improve generalization by proper gate network initialization and general domain & function decomposition.
Extensive experiments on different types of PDEs demonstrate how APINN improves the PINN and XPINN methods. Specifically, we present examples 
where XPINN performs similarly to or worse than PINN, so that APINN can significantly improve both. We also show cases where XPINN is already
better than PINN, so APINN can still slightly improve XPINN. Furthermore, we visualize the optimized gating networks and their optimization 
trajectories, and connect them with their performance, which helps discover the possibly optimal decomposition. Interestingly, if initialized
by different decomposition, the performances of corresponding APINNs can differ drastically.
This, in turn, shows the potential to design an optimal domain decomposition for the differential equation problem under consideration. 

    @article{hu2022augmented,
     title={Augmented Physics-Informed Neural Networks (APINNs): A gating network-based soft domain decomposition methodology},
     author={Hu, Zheyuan and Jagtap, Ameya D and Karniadakis, George Em and Kawaguchi, Kenji},
     journal={arXiv preprint arXiv:2211.08939},
     year={2022}
    }
